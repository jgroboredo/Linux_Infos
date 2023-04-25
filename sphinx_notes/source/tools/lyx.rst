.. _lyx-notes:

==========
LyX Notes
==========

.. epigraph:: LyX is a document processor that encourages an approach to writing based on the structure of your documents and not simply their appearance. 
              LyX combines the power and flexibility of TeX/LaTeX with the ease of use of a graphical interface. Read more in `lyx.org <https://www.lyx.org/>`_.

-------------
Configure lyx
-------------

- Tools-Preferences-File Formats: PDF (pdflatex), shortname: pdf2, Viewer: Custom - zathura
- Tools-Preferences-Output-PDF command: ``zathura --synctex-forward $$n:1:$$t $$o``
- Tools-Preferences-Shortcuts-New: buffer-view pdf2 and buffer-update pdf2
- For the spellchecker, might need to install ``hunspell-en_US`` and ``hunspel-pt_pt`` and ``enchant``
- For ``lgrenc.def not found`` -> install ``texlive-langgreek``
- To use eps figures in lyx I need ``ghostscript`` : try to ``epstopdf`` on command line to discover this.

--------
Kpathsea
--------

- ``Kpathsea`` is a library for path searching (e.g., for very quickly locating a given .sty file in a set of potentially large TEXMF trees, 
  without doing a recursive directory tree traversal every time a given file is needed. (pse -> pathsea)
- ``kpsewhich minted.sy`` to search efficiently on tex library

----------------
Configure minted
----------------

.. code-block:: bash

    sudo mkdir "/usr/share/texmf-texlive/tex/latex/minted/"
    sudo cp minted.sty "/usr/share/texmf-texlive/tex/latex/minted/"
    sudo mktexlsr

- Then in lyx, go to Tools/Tex Information, select latex styles and click rescan. minted.sty should appear in the list in lyx, go to "Tools>preferences>file handling>converters" and 
  find the converter from tex to pdflatex. Edit its command line adding the option "-shell-escape" (no quotes) into the Converter field, then click the Modify button next to the list 
  of converters. This is equivalent to going to Documents->Formats->Allow running external programs (is a better solution since it avoids writting a warning message). 
  Then click Apply in lyx, go to Document>Settings and enter "/usepackage{minted}" (no quotes) in the latex preamble in lyx, in the part of your document where you want 
  the highlighted code to appear, go to "Insert>TEX code" to get an Evil Red Text (ERT) box
- In ``Document->Settings->Listings``, add following options:

  - language=C++
  - frame=single
  - mathescape=true
  - ``syoek --synctex-forward $$n:1:$$t $$o``
- Ordered bibliography: Use style ``unsrt`` and add to preamble: ``\usepackage{notoccite}``

------------------
Install custom cls
------------------

- ``latex my_class.ins`` -> produces my_class.cls
- ``kpsewhich -var-value=TEXMFHOME`` -> prints path where to put cls
- Regarding the above command, it's good to put the usual path: ``$HOME/texmf/tex/latex/commonstuff/``
- ``kpsewhich my_class.cls`` -> to check path of the class
- Write lyx layout: In order to do this, find the basis class for our new class. For that, inspect my_class.cls and check the line LoadClass. 
  It implies that my_class.cls is a descendent of that class (let's suppose it's dependent on report class). Then, in /usr/share/lyx/layouts copy report.layout, 
  change its name to my_class.layout and edit like this:

  .. code-block:: bash

    \DeclareLaTeXClass[my_class]{name_of_layout}
    Input report.layout

- In lyx, reconfigure. Now, name_of_layout is the text we see in Document-Class
- Default classes: ``/usr/share/texmf-dist/latex/elsarticle/elsarticle.cls``