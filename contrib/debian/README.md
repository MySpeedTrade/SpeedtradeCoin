
Debian
====================
This directory contains files used to package speedtradecoind/speedtradecoin-qt
for Debian-based Linux systems. If you compile speedtradecoind/speedtradecoin-qt yourself, there are some useful files here.

## speedtradecoin: URI support ##


speedtradecoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install speedtradecoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your speedtradecoin-qt binary to `/usr/bin`
and the `../../share/pixmaps/speedtradecoin128.png` to `/usr/share/pixmaps`

speedtradecoin-qt.protocol (KDE)

