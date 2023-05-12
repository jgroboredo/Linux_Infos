.. _grub-notes:

==========
Grub Notes
==========

.. epigraph:: GRUB is a Multiboot boot loader. It was derived from GRUB, the GRand Unified Bootloader, 
              which was originally designed and implemented by Erich Stefan Boleyn.
              Briefly, a boot loader is the first software program that runs when a computer starts. 
              It is responsible for loading and transferring control to the operating system kernel software 
              (such as the Hurd or Linux). The kernel, in turn, initializes the rest of the operating system (e.g. GNU).
              
              Read more in `gnu.org <https://www.gnu.org/software/grub/>`_.

- If no update-grub command, do:
  
  .. code-block:: bash

    sudo nano /usr/sbin/update-grub
    "
    #!/bin/sh
    set -e
    exec grub-mkconfig -o /boot/grub/grub.cfg "$@" 
    "
    sudo chown root:root /usr/sbin/update-grub
    sudo chmod 755 /usr/sbin/update-grub


- If error syntax in ``grub-customizer``:

  - View -> Show placeholders
  - select entry "script code"
  - remove
- check kernel by ``uname -r``

----------------------------------------
Install grub manually when manjaro fails
----------------------------------------

.. code-block:: bash

    # Deactivate CSM in BIOS
    # Quando acaba a instalacao, ver se ele cria a particao em /boot/efi ou /boot
    sudo fdisk --list # para ver onde foi instalada a particao no pc
    sudo su
    mount /dev/sda2 /mnt # (em que sda2 era a particao com o linux)
    mount /dev/sda1 /mnt/boot/efi
    grub-install --target=x86_64-efi --efi-directory=/mnt/boot/efi --bootloader-id=manjaro --boot-directory=/mnt/boot --recheck --debug
    manjaro-chroot -a
    update-grub
    umount -R /mnt

.. note:: 
    
    Read more in: `Manjaro Forum <https://forum.manjaro.org/t/manjaro-grub-install-error-calamares-and-manual-the-why/125886>`_.