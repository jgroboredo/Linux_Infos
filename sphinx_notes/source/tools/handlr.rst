.. _handlr-notes:

============
Handlr Notes
============

.. epigraph:: handlr, written in Rust, provides the functionality of xdg-open and xdg-mime with a streamlined interface.
              Compared to xdg-utils, it includes:
              setting associations by extension, removing the need to look up or remember mime types,
              validation for mime types and extensions,
              removal of invalid entries from mimeapps.list,
              intelligent detection of mime types from file content in case filename is ambiguous,
              autocompletion of mimes, extensions, and desktop entries,
              
              Read more in `wiki.archlinux.org <https://wiki.archlinux.org/title/Default_applications#handlr>`_ and in
              `github.com <https://github.com/Anomalocaridid/handlr-regex/tree/main>`_.

------------
Installation
------------

Install the following aur packages:

- handlr-regex
- xdg-utils-handlr

-----
Usage
-----

In order to find the mime type of a given of given paths/URLs, desktop


.. code-block:: bash

    handlr mime https://duckduckgo.com . README.md # this works for directories

Then, by default, it includes shell completions for mime types and desktop files.

For example, in order to set the default file browser:

.. code-block:: bash

    handlr mime /paht/to/dir
    handlr set inode/directory pcmnanfm.desktop