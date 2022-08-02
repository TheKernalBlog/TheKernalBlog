---
published: true
---
The current version of Gnome is Gnome 40. The incredibly popular desktop is used by a lot of Linux distro’s by default, and yet for a lot of them it is only on it’s 3rd Major version. One of the biggest desktop distributions that ships with Gnome 3 is Debian. Thanks to the experimental repository in Debian 11/Sid you can install the newest version of Gnome. I am going to show you how you can enable the experimental repository and install Gnome 40. 

# Enable the Experimental Repository 

You can enable the Experimental repository by adding it to the sources.list file. The sources.list file handles all of the software repositories for apt. To add the repo, all that you need to do is open the file at /etc/apt/sources.list with your preferred text editor. Then you will want to copy-paste this line into the text file. 

	deb http://deb.debian.org/debian experimental main

Now to actually make use of it you are going to have to update the system by typing this command in the terminal. 

	sudo apt-get update && sudo apt-get upgrade

# Installing Gnome 40

Now that everything has been updated, you can finally install Gnome 40. To install most of Gnome 40, type or copy this command into the terminal. 

	sudo apt -t experimental install gnome-shell mutter gnome-backgrounds gnome-control-center gnome-applets gjs

While the install is taking place, you will be asked what display manager you would like to use. Since you are using Gnome, I would recommend selecting GDM,(Gnome Display Manager). However, there are other DM’s like LightDM, XDM, or even TBSM. 

In most cases, you are going to want to install the Gnome-session manager after everything else is installed. Simply use this command for a simple install. 

	sudo apt -t experimental install gnome-session

# Conclusion 

Now after a reboot to be safe, you should be able to login to Gnome 40. You will be able to use the bleeding edge version of Gnome while still being able to make use of the stability and apt package manager of Debian.
