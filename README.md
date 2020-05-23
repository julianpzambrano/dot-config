A minimal desktop system based on Debian GNU/Linux 10.4.0 _Buster_ - Official amd64 NETINST 20200509-10:25 i3wm and Breeze Theme

DEPENDENCIES
============

::
	sudo apt install i3 ttf-anonymous-pro gtk3-engines-breeze breeze-cursor-theme xinit xbacklight network-manager xautolock pulseaudio feh scrot zathura firefox-esr glances ranger pyhton3


SETUP
=====

::
	git clone https://github.com/julianpzambrano/dot-config.git
	cd dot-config
	git checkout i3wm
	sudo cp xinit-override.conf /etc/systemd/system/getty@tty1.service.d/
	cp bashrc ~/.bashrc
	cp i3.conf ~/.config/i3/config
	cp terminals.json ~/.config/i3/
	cp i3status.conf ~/.config/i3status/config
	sudo cp backlight.conf /etc/X11/xorg.conf.d/
	cp gtkrc-2.0 ~/.gtkrc-2.0
	cp settings.ini ~/.config/gtk-3.0/

NOTES
=====

i3 conf uses terminator as default terminal emulator, compile and config instructions on default tree of repo.
