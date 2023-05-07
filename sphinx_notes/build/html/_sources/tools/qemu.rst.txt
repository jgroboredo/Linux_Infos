.. _qemu-notes:

==========
Qemu Notes
==========

.. epigraph:: Qemu is a generic and open source machine emulator and virtualizer. Read more in `qemu.org <https://www.qemu.org/>`_.

-------------
Some Commands
-------------

.. code-block:: bash

    qemu-img create -f qcow2 qemu_image 8G
    qemu-system-x86_64 -smp 6 -m 4G -enable-kvm -cdrom arch.iso -boot order=d qemu_image
    smp (number of cores)

    qemu-system-x86_64 -soundhw ac97 -k en-us -vga std -enable-kvm -m 4G  -usbdevice tablet -smp 6 -enable-kvm -boot c qemu_image
    
    # For no sound
    qemu-system-x86_64 -k en-us -vga std -enable-kvm -m 4G  -usbdevice tablet -smp 6 -boot c qemu_image

---------
Variables
---------

.. code-block:: bash

    -k en-us (keymap)
    -usbdevice tablet

    -cpu host
    -smp 6 # number of cores
    -machine type=pc,accel=kvm
    -enable-kvm
    -format=raw ??
    -machine smm=off # bug?
    -soundhw sb16,es1370

    #telnet access
    qemu-system-x86_64 -curses -monitor telnet:127.0.0.1:1234,server,nowait -boot c qemu_image
    telnet 127.0.0.1 1234  -- in another terminal

    #KVM Quick Check
    zgrep CONFIG_VIRTIO /proc/config.gz
    lsmod | grep kvm
