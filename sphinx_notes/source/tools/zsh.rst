.. _zsh-notes:

==========
Zsh Notes
==========

.. epigraph:: Zsh is a shell designed for interactive use, although it is also a powerful scripting language
              Read more in `zsh.org <https://www.zsh.org/>`_.

-------------------
Zsh Autosuggestions
-------------------

In order to enable zsh auto-suggestions, do:

.. code-block:: bash
   
    git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
    source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh in .zshrc
    mkdir .cache/zsh && touch .cache/zsh/dirs
