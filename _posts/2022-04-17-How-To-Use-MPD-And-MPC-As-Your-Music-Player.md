---
published: true
---
You suddenly obtain a time machine. Spat back to the 90's, two items lay in front of you. A huge Dell tower running Slackware and a DVD with the band of your choice. What do you do? You start the MPD daemon and use MPC to create and listen to your playlist. What if I told you that MPD and MPC are not only still available, but also the fastest, best way to listen to music on Linux? Well, it's true, and I am going to show you how you can install, setup, and use MPD and MPC to listen to your songs using virtually no resources.

## Instillation

Installing is no issue, as MPD and MPC have been around for an extremely long time. If they are not already installed, depending on your Linux distro, copy-paste one of these commands into your terminal.

### Ubuntu/Debian

	sudo apt install mpd mpc

### Fedora/RHEL/CentOS

	sudo dnf install mpd mpc

### Arch/Artix

	sudo pacman -S mpd mpc

## Configuring

As the name suggests, MPD, the 'Music Player Daemon' requires a daemon that needs to be running all of the time. No worries though, unless you use a non-Systemd distro, you can enable it with this command.

	sudo systemctl enable mpd

Or, if you would just like to start it, and not have it run every time you boot, you can use this command.

	sudo systemctl start mpd

Then, if you would like to disable it, you can use this one.

	sudo systemctl disable mpd

## Usage

Assuming that you already have some songs in your ~/Music directory, you can use this command to pipe all of your songs into mpd like so.

	mpc ls | mpc add

Then, you can play your songs, starting with the first song alphabetically with this command.

	mpc play 1

But, if you would like some randomization, you can use this command.

	mpc random && mpc play

Then respectively, you can choose the next song,

	mpc next

pause,

	mpc pause

and stop the music.

	mpc stop

# Conclusion

While it is not the most modern solution, mpd and mpc is a great way to listen to music without having to fiddle with any bloated, resource heavy, GUI application. It not only allows you to listen to your music without Xorg, but it makes running music in the background a much less complicated, faster experience. Also, if you run LXQT, Enlightenment, XFCE, or MATE, you can rub your superior music player in the faces of GNOME and KDE users.
