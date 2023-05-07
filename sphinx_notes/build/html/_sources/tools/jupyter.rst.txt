.. _jupyter-notes:

=============
Jupyter Notes
=============

.. epigraph:: Project Jupyter is a project to develop open-source software, open standards, 
              and services for interactive computing across multiple programming languages. 
              Read more in `jupyter.org <https://jupyter.org/>`_.

-----------
Jupyter-Lab
-----------

To run over ssh, execute:

.. code-block:: bash

    ssh -L 8888(port on local):localhost::8889(port on remote) goncalo@ip jupyter-lab --no-browser --port=(same as before on remote)8889

To avoid authentication by token set a password: 

.. code-block:: bash
    
    jupyter server password

To list all active jupyter lab sessions: 

.. code-block:: bash
    
    jupyter lab list

To kill a session: 

.. code-block:: bash

    jupyter lab stop <port>
   
---------------
Troubleshooting
---------------

^^^^^^^^^^^^^^^
Opening browser
^^^^^^^^^^^^^^^

If jupyter doesn't open, do:

.. code-block:: bash

    jupyter lab build

If command above gives permission error, do:

.. code-block:: bash

    sudo chown -hR {user} {dir}
    jupyter notebook (lab) --generate-config 

Also, change ``redirect_file`` to ``false``.

Actually, this didn't work because I had to change the default browser in ``~/.profile`` to firefox.

^^^^^^^^^^^^^^^^^
Can't access file
^^^^^^^^^^^^^^^^^

This error probably happens because directory contains hidden folder .local. Do:

- set ``c.ServerApp.use_redirect_file = False`` in ``~/.jupyter jupyter_server_config.py``

- Stop server:

  .. code-block:: bash
  
      lsof -n -i4TCP:[port-number]
      kill -9 [PID]
