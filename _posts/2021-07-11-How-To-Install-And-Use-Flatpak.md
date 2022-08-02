---
published: true
---
While most people are using a package manager, or compiling from source, there is another option. Flatpaks. Flatpaks will work with almost any linux distro. They allow you to easilly install any software that isn’t in your distro’s repositories. Installing and using it is suprisingly simple. 

The first thing that you are going to have to do is install the thing. This can be done by copy/pasting these commands in your terminal. Depending on what distro that you use. 

Ubuntu/Debian: 

	sudo add-apt-repository ppa:alexlarsson/flatpak 
	sudo apt update
	sudo apt install flatpak 

RHEL/Rocky/Fedora: 

	sudo dnf install flatpak 

OpenSUSE: 

	sudo zypper install flatpak

Arch/Manjaro/Endeavour

	sudo pacman -S flatpak 

Now that you actually have Flatpak, you are going to have to add a repository. I am going to show you how to add the “Flathub” repository, because it is the most popular. However, there are others. Copy/Paste this into your terminal to do this. 

	flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

You are now ready to use Flatpak to install software. It is fairly straightforward. The first thing that you are going to have to do is find he application id of what you are trying to install. You can do this using the search command like so. 

 Flatpak search [application name] 

It will list the application ID’s of whatever software you want to install. To install it, type this command. 

flatpak install flathub [application ID] 

You are now able to install these flatpacks onto your system. While they are not the prefered way of installing software, flatpaks are great when there is somehting that just isn’t on the offical repositories.
