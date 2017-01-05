networkd-notify: desktop notification integration for networkd
==============================================================

`networkd-notify` generates desktop notifications for `systemd-networkd`
events, such as interface connection/disconnection.

The generated notifications look like::

  wlan0: configuring ...
  wlan0: online @ ESSID
  wlan0: disconnected
  ...


Usage
-----

Simply run ``networkd-notify`` at the start of your session:

  ./networkd-notify &

You'll need ``networkd`` to be running of course, and you'll also need a
notification daemon such as dunst_.


Dependencies
------------

The following software is currently required for `networkd-notify`:

- Python (3.x or 2.7)
- PyGObject/PyGI (``python-gi``)
- Python D-Bus (``python-dbus``)
- ``wireless-tools``

On Debian/Ubuntu, you can install all the required dependencies with::

  sudo apt-get install python python-gi python-dbus


Authors and Copyright
---------------------

| `networkd-notify` is distributed under GPLv3+ (see COPYING) WITHOUT ANY WARRANTY.
| Copyright(c) 2016 by wave++ "Yuri D'Elia" <wavexx@thregr.org>.

.. _dunst: http://www.knopwob.org/dunst/
