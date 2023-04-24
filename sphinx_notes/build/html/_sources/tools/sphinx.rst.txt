.. _sphinx-tricks:

=============
Sphinx tricks
=============

-------------
Nested Blocks
-------------

Consider the following example:

- List item 1 ::

   code sample

  - List item 2 ::

     code sample

In terms of code:

.. code-block:: rst

  - List item 1 ::

     code sample 1

    - List item 2 ::

       code sample 2

Basically, in this example, the "code sample 1" is indented in respect to "List item 1" 
(i.e., there are 3 spaces to the beginning of the line). On the other hand, the "code sample 2"
is indented with respect to "List item 2" (i.e, there are 3 spaces with respect to the second
indentation level, which is the hyphen where "List item 2" starts)

- List item 1 ::

    code block

  - List item 2 ::

        code block

Apparently I can simply tab the code blocks to indent. I just need to be careful where the 
nested item starts (the hyphen needs to be right under the first letter of "List item 1").

----------------------
Sphinx Doc -  extlinks
----------------------

In sphinx documentation, they have the following in the ``conf.py``:

    extlinks = {'duref': ('https://docutils.sourceforge.io/docs/ref/rst/'...}

Then, they can use, for e.g., ``(:duref:`ref <paragraphs>`)`` to link to a reference
created in the documents in the link provided (in this case, with the name paragraphs).

This extension is meant to help with the common pattern of having many external
links that point to URLs on one and the same site, e.g. links to bug trackers,
version control web interfaces, or simply subpages in other websites.  It does
so by providing aliases to base URLs, so that you only need to give the subpage
name when creating a link.

Let's assume that you want to include many links to issues at the Sphinx
tracker, at :samp:`https://github.com/sphinx-doc/sphinx/issues/{num}`.  Typing
this URL again and again is tedious, so you can use :mod:`~sphinx.ext.extlinks`
to avoid repeating yourself.

The extension adds a config value:


This config value must be a dictionary of external sites, mapping unique
short alias names to a *base URL* and a *caption*.  For example, to create an
alias for the above mentioned issues, you would add ::

    extlinks = {'issue': ('https://github.com/sphinx-doc/sphinx/issues/%s',
                        'issue %s')}

Now, you can use the alias name as a new role, e.g. ``:issue:`123```.  This
then inserts a link to https://github.com/sphinx-doc/sphinx/issues/123.
As you can see, the target given in the role is substituted in the *base URL*
in the place of ``%s``.

------------------------
Sphinx Numbered Sections
------------------------

In order to have numbered sections in sphinx, check this `link <https://sphinx-multitoc-numbering.readthedocs.io/en/latest/>`_.

The steps for installation are the following:

1. ``git clone https://github.com/executablebooks/sphinx-multitoc-numbering``
2. and install using the following commands: ::

    cd sphinx-multitoc-numbering
    sudo python setup.py install

3. Add this to the extensions list in the sphinx ``conf.py``: ::

    extensions = ["sphinx_multitoc_numbering"]

4. Finally, use ``:numbered:`` option in toctrees. 

