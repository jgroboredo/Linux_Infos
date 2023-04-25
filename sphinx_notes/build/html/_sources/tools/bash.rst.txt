.. _bash-notes:

==========
Bash Notes
==========

.. epigraph:: Bash is the GNU Project's shell - the Bourne Again SHell. Read more in `gnu.org <https://www.gnu.org/software/bash/>`_.

-----------
Bash Note 1
-----------

- The number of arguments passed to the shell script is given by ``$#``

- We identify the args passed to a script/function with ``$1, $2``, etc

-----------
Bash Note 2
-----------

The code:

.. code-block:: bash

    case $1 in
    -f|--from) command1; shift ;;
    *)         command2;;
    esac
    shift


will check if the first argument ``$1`` passed to the script matches ``-f`` or ``--from`` or any other cases; The asterisk means that it does ``command2`` if it doesn't match any of the cases above;
The ``shift`` command shifts the arguments, i.e., if I have ``$1``, ``$2`` arguments, then ``$2`` -> ``$1``.

-----------
Bash Note 3
-----------

The code:

.. code-block:: bash

    SCRIPT_DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" &> /dev/null && pwd )"

will give you the full directory name of the script no matter where it is being called from.

---------------------------
Bash Note 4 - Compare Files
---------------------------

The code:

.. code-block:: bash

    grep -F -x -v -f fileA fileB

works by using each line in ``fileA`` as a pattern (``-f fileA``) and treating it as a plain string to match (``-F``). You force the match to happen on the whole line ``-x`` and 
print out only the lines that don't match (``-v``). Therefore, you are printing out the lines in fileB that don't contain the same data as any line in ``fileA``.

---------------------------------
Bash Note 5 - Use of curly braces
---------------------------------

1) In the example:

   .. code-block:: bash
   
        var=10        # Declare variable

        echo "${var}" # One use of the variable
        echo "$var"   # Another use of the variable


   it makes no difference to use curly braces.

2) However, the ``{}`` in ``${}`` are useful if you want to expand the variable foo in the string ``"${foo}bar"`` since ``$foobar`` 
   would instead expand the variable identified by foobar.

Curly braces are also unconditionally required when:

- expanding array elements, as in ``${array[42]}``
- using parameter expansion operations, as in ``${filename%.*}`` (remove extension)
- expanding positional parameters beyond 9: ``"$8 $9 ${10} ${11}"``

---------------------------------------------
Bash Note 6 - Search recursively in directory
---------------------------------------------

- ``grep -R "stuff"`` will search recursively on all files on that directory and look for the word stuff
- ``for i in **/.ipynb_checkpoints`` will find recursively all directories with this name
- ``for i in ./pattern`` will search for this pattern in current directory
