
Debian
====================
This directory contains files used to package innoketd/innoket-qt
for Debian-based Linux systems. If you compile innoketd/innoket-qt yourself, there are some useful files here.

## innoket: URI support ##


innoket-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install innoket-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your innoketqt binary to `/usr/bin`
and the `../../share/pixmaps/innoket128.png` to `/usr/share/pixmaps`

innoket-qt.protocol (KDE)

