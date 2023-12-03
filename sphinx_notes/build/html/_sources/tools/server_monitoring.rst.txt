.. _server_monitoring-notes:

=================
Server Monitoring
=================

For the monotoring of the server, I use 3 servives: grafana, influxdb (database) and telegraf.

--------
Telegraf
--------

.. epigraph:: Telegraf is a server-based agent for collecting and sending all metrics and events 
              from databases, systems, and IoT sensors. Telegraf is written in Go and compiles into a single 
              binary with no external dependencies, and requires a very minimal memory footprint.

In order to setup telegraf, add the following to the ``docker-compose`` file:

.. code-block:: yaml

  telegraf:
    container_name: telegraf
    image: telegraf:1.28.5
    environment:
      HOST_MOUNT_PREFIX: /hostfs
      HOST_PROC: /hostfs/proc
    #devices:
    #  - /dev/vchiq  # For pi
    cap_add:
      - net_admin
    network_mode: host
    depends_on:
      - influxdb
    volumes:
      - ${CONFIG_ROOT}/telegraf/telegraf.conf:/etc/telegraf/telegraf.conf:ro
      - /var/run/docker.sock:/var/run/docker.sock:ro
      - /:/hostfs:ro
    entrypoint: /bin/bash -c
    command: >-
      "setcap cap_net_raw,cap_net_bind_service+ep /usr/bin/telegraf;
       setcap CAP_NET_ADMIN+epi /usr/bin/telegraf;
       groupadd -g $$(stat -c '%g' /var/run/docker.sock) docker;
       usermod -a -G docker telegraf;
       if [ -f /dev/vchiq ]; then chmod 666 /dev/vchiq; fi;
       exec setpriv --reuid telegraf --init-groups /usr/bin/telegraf"

The other necessary setup is just the ``telegraf.conf``. Note the ``influxdb`` url: ``http://localhost:8086``.
This is required since telegraf is running in ``network_mode: host``.

Finally, just setup the ``organization`` and ``bucket`` for InfluxDB as:

- organization = "xeon-metric"
- bucket = "telegraf"

--------
InfluxDB
--------

.. epigraph:: InfluxDB is an open-source time series database developed by the company InfluxData. 
              It is used for storage and retrieval of time series data in fields such as operations 
              monitoring, application metrics, Internet of Things sensor data, and real-time analytics. 
              It also has support for processing data from Graphite.
              Read more in `influxdata.com <https://www.influxdata.com/>`_.

In order to setup InfluxDB, add the following to the ``docker-compose`` file:

.. code-block:: yaml

  influxdb:
    container_name: influxdb
    image: influxdb:2.7.4
    env_file: .env
    user: ${PUID}:${PGID}
    environment:
      INFLUXDB_REPORTING_DISABLED: 'true'
    volumes:
      - ${CONFIG_ROOT}/influxdb/config:/etc/influxdb2
      - ${CONFIG_ROOT}/influxdb/data:/var/lib/influxdb2
    ports:
      - 127.0.0.1:8086:8086

For the first time, in order to setup the database, set ``ports`` to ``8086:8086`` to be accessible outside the server.

Then, the necessary things to keep in mind are:

- Set the organization to match whatever is used in the other services: "xeon-metric";
- Set the bucket to match whatever is used in the other services: "telegraf";
- Save the token to be used both by telegraf and grafana.

-------
Grafana
-------

.. epigraph:: Grafana open source software enables you to query, visualize, alert on, 
              and explore your metrics, logs, and traces wherever they are stored. 
              Grafana OSS provides you with tools to turn your time-series database (TSDB) 
              data into insightful graphs and visualizations. The Grafana OSS plugin 
              framework also enables you to connect other data sources like NoSQL/SQL 
              databases, ticketing tools like Jira or ServiceNow, and CI/CD tooling 
              like GitLab.

In order to setup grafana, add the following to the ``docker-compose`` file:

.. code-block:: yaml

    grafana:
      container_name: grafana
      image: grafana/grafana:10.2.2
      env_file: .env
      depends_on:
        - influxdb
      user: ${PUID}:${PGID}
      environment:
        - "GF_SERVER_ROOT_URL=%(protocol)s://%(domain)s:%(http_port)s/grafana/"
      volumes:
        - ${CONFIG_ROOT}/grafana:/var/lib/grafana
      ports:
        - 127.0.0.1:3000:3000

The first login user and password are "admin:admin".

Assuming ``influxdb`` is already setup, go to data sources and add ``influxdb`` with the following parameters:

^^^^^^^^^^^^^^^
InfluxDB - Flux
^^^^^^^^^^^^^^^

- Query Language: Flux
- Url: ``http://influxdb:8086``
- Basic Auth: Disabled
- InfluxDB details:
  
  - Organization: xeon-metric
  - Token: token from influxdb
  - Default bucket: telegraf (created by me)
  - Min time interval: 10s (default)
  - Max series: 1000 (default)

After clicking "Save & test", it should recognize 3 buckets.

^^^^^^^^^^^^^^^^^^^
InfluxDB - InfluxQL
^^^^^^^^^^^^^^^^^^^

In InfluxDB, do the following:

.. code-block:: bash

    docker exec -u 0 -it influxdb bash

    # To try:
    influx config create --active -n <config name> -u http://influxdb:8086 -t <token> -o xeon-metric # -o org_id
    influx v1 dbrp create --db <db_name> --rp autogen --bucket-id <bucket_id> --default

    # However, I should be able to use virtual dbrp mappings
    # Check with:
    influx v1 dbrp list

    # The above command outputs a telegraf database (with the same id as the bucket I created)

After, in datasources, add the following:

- Query Language: InfluxQL
- Url: ``http://influxdb:8086``
- Add custom header: 
  
  - Header: Authorization
  - Value: Token <token_here>

- Database: telegraf (same as in ``influx v1 dbrp list``)
- User: goncalo
- Pw: <pw>
- Get
- Min time interval: 10s (default)
- Max series: 1000 (default)