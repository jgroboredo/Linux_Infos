.. Gonçalo's Personal Notes documentation master file, created by
   sphinx-quickstart on Sun Apr 16 15:05:38 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

======================================
Welcome to Gonçalo's Personal Notes's!
======================================

These notes are written using sphinx. For more information, visit the sphinx documentation `here <https://www.sphinx-doc.org>`_.
In order to build the notes, just run ``make clean; make html``.

The dependencies to build this documentation are:

- sphinx;
- furo (theme);
- sphinx-multitoc-numbering - check :ref:`this section <sphinx-numbered-sections>` for more information;
- sphinx-copybutton - visit `link <https://sphinx-copybutton.readthedocs.io>`_ for more information.

In order to install the dependencies, simply run ``pip install -r requirements.txt``.

.. note:: 

   Note that we should use a ``venv`` in order to build this. In order to do so:

   .. code-block :: bash

      python -m venv python-sphinx
      source python-sphinx/bin/activate

   An even better solution is to use ``pyenv`` and ``pyenv-virtualenv`` (the latter found on aur) to manage
   virtual environments. 
   To do so, after installing the packages, add the following lines to ``.zshrc``:

   .. code-block :: bash

      export PATH="$HOME/.pyenv/bin:$PATH"
      eval "$(pyenv init -)"
      eval "$(pyenv virtualenv-init -)"
   
   After, on the project folder, simply do:

   .. code-block :: bash

      pyenv virtualenv <optional_python_version> project_name
      pyenv local project_name # on the base folder of the project

   After this, ``which python`` should point to ``$HOME/.pyenv/shims/python`` and 
   ``pyenv versions`` should show the correct virtualenv selected. 
   From now on, simply use ``python -m pip install <package>`` to do stuff.

--------
Contents
--------

.. toctree::
   :maxdepth: 2
   :caption: Contents:
   :numbered:

   tools/sphinx
   tools/git
   tools/bash
   tools/lyx
   tools/qemu
   tools/inkscape
   tools/zathura
   tools/zsh
   tools/jupyter
   tools/pacman
   tools/grub
   tools/vim
   tools/python
   tools/libreoffice
   tools/vscode
   tools/nvidia
   tools/linux_sound
