.. _code-notes:

==========
Code Notes
==========

.. epigraph:: The repository ("Code - OSS") is where Microsoft develops the Visual Studio Code product 
              together with the community. Not only do they work on code and issues there, they also publish 
              our roadmap, monthly iteration plans, and endgame plans. The source code is available to everyone 
              under the standard MIT license.

              Read more in `github.com <https://github.com/microsoft/vscode>`_.

------------
Installation
------------

In archlinux, install the following packages:

.. code-block:: bash
   
   pacman -S code # Code - OSS — Official Arch Linux open-source release.
   yay -S code-features
   yay -S code-marketplace

----------
Extensions
----------

^^^^^^^^^^^^^^^
C/C++ Extension
^^^^^^^^^^^^^^^

In settings, set the ``C_Cpp.default.configurationProvider`` to ``ms-vscode.cmake-tools``.

^^^^^^^^^^^
CMake Tools
^^^^^^^^^^^

In settings, set the ``cmake.configueOnOpen`` to ``false``.

^^^^^^^
GitLens
^^^^^^^

By clicking on the ``GitLens`` extension on the left hand bar, I can then select ``file history``
and check the history of the current open file.

^^^^^^^^^
SonarLint
^^^^^^^^^

By clicking on the ``SonarLint`` extension on the left hand bar, I can then select connected mode 
and add a ``SonarQube`` connection. The token should be a UserToken and not a ProjectAnalysis token.
At least the latter was not working when setting up ``SonarLint``.

This can also be debugged by clicking ``Ctrl + Shift + P`` , then select ``Show Logs``.

