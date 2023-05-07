.. _zathura-notes:

=============
Zathura Notes
=============

.. epigraph:: Zathura is a highly customizable and functional document viewer. 
              It provides a minimalistic and space saving interface as well as an 
              easy usage that mainly focuses on keyboard interaction.
              Read more in `pwmt.org <https://pwmt.org/projects/zathura/>`_.

To install zathura, run:

.. code-block:: bash

    pacman -S zahtura-pdf-poppler

In order to make ``zathura`` default pdf viewer:

.. code-block:: bash

    mimeo --add application/pdf zathura.desktop

To discover the real name of zathura.desktop run:

.. code-block:: bash

    locate zathura.desktop

To check that pdf files have the correct mimetype run:

.. code-block:: bash

    mimeo -m pdf_file.pdf

To activate clipboard add ``set selection-clipboard clipboard`` to ``~/.config/zahtura/zathurarc`` or ``/etc/zathurarc``
