.. _libreoffice-notes:

=================
Libreoffice Notes
=================

.. epigraph:: LibreOffice is Free and Open Source Software. Development is open to new talent 
              and new ideas, and our software is tested and used daily by a large and devoted 
              user community. 
              Read more in `libreoffice.org <https://www.libreoffice.org/>`_.

---------------------
Libreoffice - General
---------------------

- Latex in impress: ``pacman -S libreoffice-extension-texmaths``
- Check extension in Extension Manager inside ``libreoffice``
- To install ``ExpandAnimations`` go to ``Tools->ExtensionManager`` and add there the oxt file

---------------
Fail to startup
---------------

If ``libreoffice`` fails to startup, try to launch it in safe mode and disable hardware acceleration:

.. code-block:: bash

    libreoffice --safe-mode

And then Select "Configure" -> "Disable Hardware Acceleration (OpenGL, OpenCL)".