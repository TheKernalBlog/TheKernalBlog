---
published: true
---

I know that there are a lot of people that love hopping desktop environments. I have probably tried almost all desktop environments. So I am going to collect some of the most popular desktops, and show you how to install them on debian, RHEL, and Arch based systems. Depending on what distro you use, you can simply copy-paste these commands to get your preferred desktop environment. 

## XFCE

Debian: 

	sudo apt-get install xfce4

Arch:

	sudo pacman -S xfce4

RHEL: 

	sudo dnf install @xfce-desktop-environment

## LXDE

Debian 

	sudo apt-get install lxde

Arch: 

	sudo pacman -S lxde 

RHEL: 

	sudo dnf install @lxde-desktop-environment 

## LXQT

Debian: 

	sudo apt-get install lxqt

Arch: 

	sudo pacman -S lxqt

RHEL: 

	sudo dnf install @lxqt-desktop-environment 

## Cinnamon 

Debian: 

	sudo apt-get install cinnamon 

Arch: 

	sudo pacman -S cinnamon 

RHEL: 

	sudo dnf install @cinnamon-desktop-environment


## MATE

Debian: 

	sudo apt-get install mate

Arch: 

	sudo pacman -S mate

RHEL:

	sudo dnf install @mate-desktop-environment 

## KDE-Plasma 

Debain:

	sudo apt-get install task-kde-desktop

Arch: 

	sudo pacman -S xorg plasma plasma-wayland-session kde-applications 

RHEL: 

	sudo dnf install @kde-desktop-environment 

## Gnome 

Debain: 


	sudo apt-get install gnome 

Arch: 

	sudo pacman -S gnome 

RHEL: 

	sudo dnf group install “GNOME Desktop Environment”

And now, by copy-pasting these commands, you should be able to use any desktop environment that you want. Or, you could install all of them and keep them all on your system. I’m not your boss. But I do hope that this helped you.
