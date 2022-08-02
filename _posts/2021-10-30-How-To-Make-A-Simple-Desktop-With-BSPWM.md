---
published: true
---
Many Linux users opt to use a window manager instead of a desktop environment. Especially tiling window managers. One of the best tiling window managers is BSPWM. It is a very minimalistic window manager that can be a little hard to set up, which is why I am going to give a guide on how to get a very basic BSPWM with working keyboard shortcuts, compositing, and a wallpaper. 

# Installing everything 

While you might think that you only would need to install BSPWM itself, you are going to have to install a few things to get it to work. Nitrogen for the wallpaper, sxhkd for keyboard shortcuts,  picom for the compositor, and of course, BSPWM. This guide also assumes that you have a text editor and a terminal emulator of your choice. Depending on what distro you use, simply copy-paste one of these commands into your terminal. 

Ubuntu/Debian: 

	sudo apt install nitrogen sxhkd picom bspwm

# Arch/Manjaro 

	sudo pacman -S nitrogen sxhkd picom bspwm

# Fedora

	sudo dnf install nitrogen sxhkd picom bspwm

# OpenSUSE

	sudo zypper install nitrogen sxhkd picom bspwm 

This should also pull a few dependencies like dmenu. 

# Making the directories and copying the config files

First, you are going to want to make some directories to put the config file. Put these two commands in your terminal. 

	mkdir ~/.config/bspwm

	mkdir ~/.config/sxhkd
	
Then you are going to need to move the config files from their place in /usr/share/doc/bspwm/examples to the config directories that you just made. This can be acheived using these two commands in the terminal. 

	sudo mv /usr/share/doc/bspwm/examples/bspwmrc ~/.config/bspwm

	sudo mv /usr/share/doc/bspwm/examples/sxhkdrc ~/.config/sxhkd 


Now BSPWM is at a space where it is almost ready to be used. But there are still some things to do. 

# Using your correct terminal emulator 

Unless you only want to use the default terminal emulator, you are going to want to edit the sxhkd file. Make sure that you open with root permissions like this. 

	sudo (Text Editor) ~/.config/sxhkd/sxhkdrc 

Around the top of the file you will see a key binding called “Terminal Emulator”. Remove the terminal emulator that is there and replace it with the terminal emulator that you would like to use. 

# Adding the wallpaper and compositing 

Launch nitrogen, then add the directory where your wallpaper is. Click apply, and you should see that the wallpaper is applied. Now, to get it to save everytime that you open BSPWM you need to add it to bspwmrc. Remember also to open this one with root privlages. 

	sudo (Text Editor) ~/.config/bspwm/bspwmrc

You are going to need to add nitrogen --restore & to your bspwmrc. Plus, if you want to have compositing, add picom & to the bspwmrc as well. This will autostart these both at login. 

# Conclusion 

If you have followed this guide, you should now have a very simple BSPWM desktop. While there is still much more to do, and much more to lean with BSPWM, this guide should allow you to set up a base for you to build upon if you want to use BSPWM.
