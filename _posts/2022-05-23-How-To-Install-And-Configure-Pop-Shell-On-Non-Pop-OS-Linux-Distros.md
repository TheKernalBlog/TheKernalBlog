---
published: true
---
For the longest time, I used tiling window managers. They are super snappy, easy to learn, and just worked a lot better for my workflow. And yet, loving GNOME, LibAdwiata, and GTK, I finally decided to make the switch, especially since I have better hardware. One of the things that has made the transition especially easy, is Pop-Shell. Pop-Shell, is a GNOME extension working on every current GNOME version, designed for Pop_OS!, that features tiling windows, and a Rofi-like application menu that can help mimic the feel of traditional tiling window managers. And so, because not everyone wants to use Pop_OS!, I am going to show you how you can not only install the Pop-Shell extension, but install and configure the launcher, so that you can have the amazing experience with tiling on GNOME. 

# Installing the extension

### Ubuntu/Debian 

In order to make sure that Pop-Shell works seamlessly on Ubuntu or Debian, you need to build from source like so. 

	sudo apt install node-typescript make

	git clone https://github.com/pop-os/shell

	cd shell 

	make local-install

### Fedora

Pop-Shell is available in the official Fedora repositories, so installing is as simple as using this one command. 

	sudo dnf install gnome-shell-extension-pop-shell


### Arch Linux 

Pop-Shell, like most things, is available in the AUR. So, depending on your AUR helper, just install like so. 

	AURHELPER -S pop-shell

# Installing Pop-Launcher

You will find, that despite having the extension, when you try to open up the launcher, although it appears, you can't use it to search for or launch applications. Because, in order for the launcher to work, you need Pop-Launcher. So, unless you are going to ignore it and use the default GNOME launcher, simply install using any number of these commands keeping your distro into consideration. 

## Installing Dependencies  

### Ubuntu/Debian

	sudo apt install just rust cargo 

### Fedora

	sudo dnf install just rust cargo

### Arch 

	sudo pacman -S just rust cargo 

## After Dependencies Are Installed 

	cd launcher 

	just 

	just install

# Remaping Pop-Launcher To Super Key (This Will Remove Overview Shortcut) 

This is a purely optional thing, that I would not recommend you do if you use the GNOME overview a lot. But, if you would like to use the Pop-Laucher as your primary launcher, you should install [this](https://extensions.gnome.org/extension/4797/pop-launcher-super-key/) extension. This will bind your super key to the launcher. And while you can do a similar thing using gsettings, it will make all keyboard shortcuts that require the super key useless, which is a big problem for Pop-Shell, so I would advise against it. 

# You did it!! 

You have successfully installed Pop-Shell and by extension, the Pop-Launcher, giving you the ability to use GNOME, on any Linux distro, as a tiling window manager. This allows you to get the same productivity boost you would otherwise get installing a tiling window manager, without half the effort, and with the ability to seamlessly integrate with GNOME applications. And plus, you get to scoff at KDE users, which is always a pro.
