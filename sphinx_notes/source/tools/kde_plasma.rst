.. _kde_plasma-infos:

==================================
KDE Infos - Notes on configuration
==================================

.. epigraph:: KDE Plasma, a graphical desktop environment with customizable layouts and panels, 
              supporting virtual desktops and widgets. Written with Qt 5 and KDE Frameworks 5. KDE Frameworks, a collection of libraries and software frameworks built on top of Qt.
              Read more in `kde.org <https://kde.org/plasma-desktop/>`_.

--------
Packages
--------

The list of relevant packages is:

* plasma-desktop
* plasma-wayland-session
* plasma-workspace-wallpapers
* plasma-systemmonitor
* plasma-nm
* plasma-pa
* plasma-browser-integration
* powerdevil
* bluedevil
* kdialog  # for native dialogs in some apps
* breeze breeze-gtk
* kwrited
* phonon-qt5-gstreamer
* kde-gtk-config
* xdg-desktop-portal xdg-desktop-portal-kde xdg-desktop-portal-gtk
* khotkeys

----------
Launch env
----------

.. code-block:: bash

    # Wayland
    export MOZ_ENABLE_WAYLAND=1
    export XDG_SESSION_TYPE=wayland
    exec startplasma-wayland

    # X11 
    exec sx startplasma-x11

---------
Autostart
---------

Check the following paths:

* ``~/.kde/Autostart``
* ``~/.kde/share/autostart``
* ``~/.config/autostart``
* ``~/.local/share/autostart``
* ``/etc/xdg/autostart``
* ``/usr/share/autostart``

-------------------------
XDG Autostart directories
-------------------------

Place Desktop entries (i.e. .desktop files) in the appropriate **XDG Autostart directory**:

- user-specific: ``$XDG_CONFIG_HOME/autostart`` (``~/.config/autostart`` by default)
- system-wide: ``$XDG_CONFIG_DIRS/autostart`` (``/etc/xdg/autostart`` by default)

To disable a system-wide entry, create an overriding entry containing ``Hidden=true``.

-----------------
Autostart Manager
-----------------

The program scans ``$HOME/.config/autostart/`` for applications and login scripts, ``$HOME/.config/plasma-workspace/env``
for pre-startup scripts and ``$HOME/.config/plasma-workspace/shutdown`` for logout scripts to check what programs and 
scripts are already there and displays them. However, applications in ``/etc/xdg/autostart`` are also launched.

To autostart an application, navigate to ``System Settings > Startup and Shutdown > Autostart`` and add the program or 
shell script of your choice. For applications, a ``.desktop`` file will be created, for login scripts, a ``.desktop``
file launching the script will be created.

If a desktop file under ``$HOME/.config/autostart/`` has ``OnlyShowIn=XFCE;``, then it will not be autostarted.

------------------
Disable kdeconnect
------------------

First we need to avoid kdedconnect to autostart:

.. code-block:: bash
    
   cp /etc/xdg/autostart/org.kde.kdeconnect.daemon.desktop ~/.config/autostart/

Now edit the file ``~/.config/autostart/org.kde.kdeconnect.daemon.desktop`` and add ``Hidden=true``. 
Actually you can even remove everything else, because only the file name has to be identically so it's "overriden". So it looks like:

.. code-block:: text
   
   [Desktop Entry]
   Hidden=true

Now the autostart service is disabled, but this isn't enough. We also need to "disable" the d-bus service:

.. code-block:: bash
   
   mkdir -p ~/.local/share/dbus-1/services/
   cp /usr/share/dbus-1/services/org.kde.kdeconnect.service ~/.local/share/dbus-1/services/


Edit the file ``~/.local/share/dbus-1/services/org.kde.kdeconnect.service``  and change Exec to ``/usr/bin/false`` so the file looks like:

.. code-block:: text

   [D-BUS Service]
   Name=org.kde.kdeconnect
   Exec=/usr/bin/false


``/usr/bin/false`` will return with a "error" return code (because it returns with 1 and not 0), so your logs (via journalctl) 
may display the process couldn't start or failed. But that shouldn't matter.

Now kdeconnectd should not run anymore after you logout and login again.


----------------------------------
Fixing hanging service on shutdown
----------------------------------

First atempt: ``sudo rm /usr/share/dbus-1/accessibility-services/org.a11y.*``

Add:

``NoExtract = usr/share/dbus-1/accessibility-services/org.a11y.*``

to makepkg.conf.

----------------------
Settings Configuration
----------------------

^^^^^^^^^^^^^^^^^^^^^^^^^^
Shortcuts and Key Bindings
^^^^^^^^^^^^^^^^^^^^^^^^^^

- "Switch to Next Screen" shortcut to work: you need to check "Separate screen focus" option first from System settings → Window behavior → Window Behavior (on the left side) → Separate screen focus
- Logout Menu: Shortcuts → Session Management → Logout (default: ctrl+alt_del)
- Screen Lock: Workspace Behavior → Sreen Locking (also, disable automatic screen lock here)
- "Switch to Screen 0": Meta+Ctrl+Right
- "Switch to Screen 1": Meta+Ctrl+Left
- "Switch to Window to the Left": Meta+Alt+Left
- "Switch to Window to the Right": Meta+Alt+Right
- Window Management -> Window Behavior -> Focus follows mouse; Delay focus by: 0ms;
- Window Management -> Window Behavior -> Window Actions -> Meta + Middle Click: Minimize;
- Window Management -> Task Switcher -> Filter windows by -> Screens -> Current Screen (basically, apply this to each one of the settings;
- Window Management -> Virtual Desktops -> Add more desktops;
- Keyboard -> Shortcuts -> Close Window -> Meta + Shift + Q
- Keyboard -> Shortcuts -> Make Window Full Screen -> Meta + Shift + F
- Keyboard -> Shortcuts -> Maximize Window -> Meta + F
- Keyboard -> Shortcuts -> Remove all Quick Tile settings
- Keyboard -> Shortcuts -> plasmashell -> Remove all Activate Task Manager Entry
- Keyboard -> Shortcuts -> Set Switch to Desktop shortcuts
- Keyboard -> Shortcuts -> Add new -> Firefox Web Browser (Meta + F2)
- Keyboard -> Shortcuts -> Add new -> Alacritty (Meta + Enter)
- Keyboard -> Shortcuts -> Add new -> -> command -> ``albert toggle`` (Meta + D)
- In polonium settings, add albert to filter process

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Startup and Shutdown: Background Services
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Remove Search Folder Updater (also go to Search → File Search and untick ``Enable File Search`` to completely disable file search).

Otherwise, search for ``file search`` and do:

- File indexing: enabled;
- Data to index: files names only;
- Specifically add folders to index - eventually disable the entire home folder.

In order to disabel discover service,

.. code-block:: bash

   sed -e '$aHidden=True' /etc/xdg/autostart/org.kde.discover.notifier.desktop > "$HOME/.config/autostart/org.kde.discover.notifier.desktop" 

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Startup and Shutdown: Desktop Session
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- [x] Start with an empty session
- [x] Confirm Logout
- [x] Offer Shutdown Options
- [x] End Current Session

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Power Management: Energy Saving
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Untick Screen Energy Saving

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Display and Monitor: Night Color
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Activate

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Window Management: Task Switcher
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Filter Windows by: Virtual desktops and Screens (**current** in both)

^^^^^^^^^
FlameShot
^^^^^^^^^

I should not use the shortcut option for flameshot that comes by default. Instead do:

- Go to Settings > Shortcuts > Custom Shortcuts
- Right click > New > Global Shortcut > Command/Url
- Select trigger and Command/Url to ``/usr/bin/flameshot gui``

If flameshot compresses both monitors, check if they are both with 100% scalling. 

If flameshot only appears in one monitor, create the following window rule (Settings -> Window Management -> Window Rules):

- Name: Force Flameshot size
- Window Class: Exact Match -> flameshot
- Match whole window class: No
- Window types: Normal Windows
- Add property -> Window Title: Exact match -> Flameshot
- Add property -> Position -> Force -> 0x0
- Add property -> Fullscreen -> Force -> No
- Add property -> Obey geometry restrictions -> Force -> No
- Add property -> Keep above other windows -> Force -> Yes

^^^^^^^^
Task Bar
^^^^^^^^

- Add "Task Manager" widget to each panel
- Right-click on an item in Task Manager -> Configure Task Manager
- Behavior tab -> Filter: Show only tasks from the current screen

^^^^^^^^
Polonium
^^^^^^^^

- Go to `GitHub <https://github.com/zeroxoneafour/polonium/releases/>`_ and download the polonium.kwinscript asset from a release of your choice, then install it in KWin Scripts in the settings menu (or use yay);
- If using yay, run ``yay -S kwin-polonium``;
- In order to activate, go to ``Settings -> KWin Scripts -> Polonium``;
- In ``Polonium`` settings, change ``Insetion point`` to ``Right Side``;