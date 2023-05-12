.. _pacman-notes:

=============
Pacman Notes
=============

.. epigraph:: The pacman package manager is one of the major distinguishing features of Arch Linux. 
              It combines a simple binary package format with an easy-to-use build system. 
              The goal of pacman is to make it possible to easily manage packages, 
              whether they are from the official repositories or the user's own builds.
              Read more in `arch wiki <https://wiki.archlinux.org/title/pacman>`_.



- Update pacman mirrors: ``reflector --verbose --latest 5 --sort rate --save /etc/pacman.d/mirrorlist``
- Check recently installed packages: ``grep -i installed /var/log/pacman.log``

------------
Pacman cache
------------

.. code-block:: bash
    
    sudo ls /var/cache/pacman/pkg/ | wc -l # checks cached packages
    du -sh /var/cache/pacman/pkg/ # disk space occupied by cache
    sudo paccache -r # cleans all packages except most recent 3
    sudo paccache -rk 1 # keep only one most recent version
    sudo pacman -Sc # remove all uninstalled packages
    sudo pacman -Scc # remove installed and uninstalled packages from cache
    sudo paccache -ruk0 #**** remove all versions of uninstalled packages
    change /etc/pacman.conf ParallelDownloads=5

---------------------
Install from live usb
---------------------

.. code-block:: bash

    mount system: mount /dev/sdax /mnt
    sudo pacman --root /mnt -S package
    sudo pacman -Qkk | grep warning # To verify the presence of the files  installed by a package
    sudo pacman --root /mnt -S $(sudo pacman --root /mnt -Qeq) --noconfirm # reinstalls installed packages
    #If need to remove aur packages:
    sudo pacman --root /mnt -Qeq > packages.txt
    sudo pacman --root /mnt -S $(cat packages.txt) --noconfirm

------------
Pacman infos
------------

.. code-block:: bash

    pacman -Qe # lists explicitly installed packages
    pacman -Rsc # uninstalls (including unneeded dependencies)
    pacman -Qs "query" # search installed packages for keywords
    pacman -Qdt # list unneeded packages
    pacman -Rns $(pacman -Qdtq) # uninstall unneeded packages (nota: quando adicionei isto aos aliases, sempre que abri o terminal pedia-me a pass do sudo (estava a correr o que esta a frente de $)

--------------
Pacman mirrors
--------------

.. code-block:: bash

    sudo pacman-mirrors --fasttrack && pacman -Syyu
