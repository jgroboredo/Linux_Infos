.. _vim-notes:

==========
Vim Notes
==========

.. epigraph:: Vim is a highly configurable text editor built to make creating and changing 
              any kind of text very efficient. It is included as "vi" with most UNIX systems and with Apple OS X. 
              Read more in `vim.org <https://www.vim.org/>`_.

-----------
Install Vim
-----------

- ``yay -S vim-plug-git``
- add ``.vimrc`` with the plugs I want
- add folder ``~/.vim/plugged/``
- to install plugs, do ``:PlugInstall``
- for fzt pluggin: ``:Files`` command
- For the NERDTree plugin to see icon of file, install: ``yay -S nerd-fonts-complete`` ;
  This font package my screw up font sizes of icons. To correct this, add to i3blocks config the following:

  .. code-block:: text
    
     <span size='small' font_weight='light'> icon </span> 

  And change font on terminal to SauceCodePro Nerd Font Medium

- To open a file in a new tab in ``nerdtree``, press ``t`` (or ``T``); to open vertically click ``s`` ;
- To cycle through windows: ``C-W-W``, ``C-W-H``, ``C-W-L``, ``C-W-J``, ``C-W-K``
- To open file using fzf do:
- ``CTRL+T`` to open in new tab
- ``CTRL+X`` to open a new split
- ``CTRL+V`` to open in a new vertical split
- While in NERDTree, click on "m" to have a menu to do stuff with the file or other things
- ``yay -S vim-youcompleteme-git`` -> vim autocompletion (Needs to be done separately from the installation of the dotfiles)
- No need to add this plugin (``vim-youcompleteme-git``) to the ``.vimrc`` file
- add: ``let g:ycm_show_diagnostics_ui = 0`` to disable error checking by ``YouCompleteMe``
- ``pacman -S python-black``

----------------------
Install Vim in cluster
----------------------

.. code-block:: bash

    git clone https://github.com/vim/vim.git
    ./configure --prefix=$HOME/.local && make && make install
    # More flags: --disable-perlinterp --enable-rubyinterp --enable-multibyte --enable-pythoninterp --with-features=huge
    export PATH="/home/youruser/.local/bin:$PATH"
    # For plugins:
    mkdir .vim/autoload
    curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim


Place in ``.vimrc`` before ``plug#begin()`` :

.. code-block:: text

    let data_dir = has('nvim') ? stdpath('data') . '/site' : '~/.vim'
    if empty(glob(data_dir . '/autoload/plug.vim'))
        silent execute '!curl -fLo '.data_dir.'/autoload/plug.vim --create-dirs  https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
        autocmd VimEnter * PlugInstall --sync | source $MYVIMRC
    endif

------------
Vim snippets
------------

- ``:UltiSnipsEdit`` command opens up a custom snippets file for the current ``language/filytype``
- Don't need the above step if I install ``vim-snippets`` plugin

-----------
Manage Tabs
-----------

- To move tabs -> ``Alt + arrows``
- To merge tabs -> ``Ctr + m`` or ``Ctrl + n`` ;
- To exchange position of merged tabs -> ``<C-w> x`` ;
- To change cursor position -> ``<C-w> w`` ;
- To rotate windows -> ``<C-w> <C-r>``

----------------
Vim surroundings
----------------

- cs(atual)(target) -> change surround from "atual" to "target"
- ds"  -> delete surround "
- ysiw[ -> yank surround inner word [ -> puts [ surrounding the word the cursor is in
- ysf(smth)[ -> puts [ surrounding current cursor position till smth

-------------
Some commands
-------------

- procurar coisas: ``/searchthing`` e usa-se n ou N para avançar para as seguintes
- procurar string e substituir:
  
.. code-block:: text

  :s/search/replace/
  :8,10 s/search/replace/g procura nas linhas 8 a 10
  :%s/search/replace/g procura no documento inteiro
  :%s/search/replace/gc pede confirmação para alterar

- copiar e colar: selecionar o texto, y copia, p cola