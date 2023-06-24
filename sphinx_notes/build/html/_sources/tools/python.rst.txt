.. _python-notes:

============
Python Notes
============

.. epigraph:: Python is a high-level, general-purpose programming language. 
              Its design philosophy emphasizes code readability with the use of 
              significant indentation via the off-side rule. Python is dynamically 
              typed and garbage-collected. 
              
              Read more in `python.org <https://www.python.org/>`_.

-----
pyenv
-----

Use ``pyenv`` to manage python versions. Check the installation instrctions in  
`github.com <https://github.com/pyenv/pyenv>`_. 

For ``zsh`` do:

.. code-block:: bash

    echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
    echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
    echo 'eval "$(pyenv init -)"' >> ~/.zshrc

- Then, the installed versions can be checked with ``pyenv versions`` and the version in use
  using ``pyenv version``.
- In order to change the python version used for the current shell: ``pyenv shell <version>``.
- To install a new version, we can check the available versions with ``pyenv install --list``
  and then ``pyenv install <version>``.

^^^^^^^^^
pyenv pip
^^^^^^^^^

After changing the python version, we can simply use `pip` and it will automatically install packages
for that python version. The same is true to initialize a new venv: ``python -m venv <venv_name>``
will work.



