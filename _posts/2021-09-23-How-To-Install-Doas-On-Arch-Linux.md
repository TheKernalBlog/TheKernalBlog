---
published: true
---
If you are like me, you value speed over much else. While sudo is great, Doas is an alternative to sudo that is faster and has a cleaner codebase. If you would like the utility of sudo with a more speedy and less bloated experience, I am going to show you how you can install and use Doas on an Arch Linux machine. 

# 1. Installing Doas 

I prefer to use the AUR to install Doas. Assuming that you use the yay AUR helper, simply put this command into your terminal. 

	yay -S doas

# 2. Adding yourself to the config file 

After you install Doas, you will notice that it does not work. If you try to use it as an alternative to sudo, it will do nothing, which is why you are going to have to edit a config file. The config file is located at /etc/doas.conf . Make sure that you open with root privileges. As an example, I am going to show you how to do it using the su command. 

	su – root

Then enter your password. Now, you are going to have to edit the file in your favorite text editor. 

	<NAMEOFEDITOR> /etc/doas.conf

You will find it empty. Assuming that you are a part of the wheel group, it makes more sense to use wheel instead of your user because then you will be able to add more users without having to edit the config file. Simply copy/paste this line into the file. 

	permit :wheel

All that there Is left to do is save the file and exit. You can now start using doas. 

# Usage

You can use doas like you would sudo. Entering it before a command will prompt you for a password and allow you to run it with root privileges. An example would be using it to update the system with pacman like this. 

	doas pacman -Syu

# Conclusion 

Doas was a great addition by the OpenBSD team and is great on Linux. If you are looking to build your own non-bloated and fast machine I would recommend that you install doas instead of sudo. Not only is it simpler, it is super fast and takes up almost no disk space.
