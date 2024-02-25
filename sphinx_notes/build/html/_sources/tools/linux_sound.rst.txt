.. _linux_sound-notes:

====================
Sound on Linux Notes
====================

Currently, my sound setup relies on `PipeWire <https://wiki.archlinux.org/title/PipeWire>`_ together with 
``pamixer`` to control the outputs, volume, toggle mute, etc.

-----------------------------
Line-in jack for 7.1 surround
-----------------------------

First, install ``aslsa-tools``.

Then, using ``hdajackretask``, select ``Realtek ALC897`` and set:

- Pink Mic, Rear Side, Pin ID 0x18 override - Line out (Center LFE);
- Blue Line In, Rear Side, Pin ID:0x1a override - Line out (Back).

This can then be tested using:

.. code-block:: bash

   speaker-test -t wav -c 6 -l 1


