---
published: true
---

Gnome is great. It changes your workflow, and can be really good for someone who uses their keyboard a lot. However, it doesn’t’ give you a lot of options to customize out of the box. I am going to go over how you can change icons, themes, window buttons, and how to utilize extensions to customize your desktop to the max.

To do basically any customization you are going to have to get “gnome-tweak-tool”. It is a tool that does exactly what it says. It allows you to completely change your gnome desktop.  To install it, you can type these lines into your terminal depending on what distro that you use. 

Ubuntu-Debian 

	sudo apt-get install gnome-tweak-tool

Arch-Manjaro

	sudo pacman -S gnome-tweak-tool

Fedora/RHEL

	sudo dnf install gnome-tweak-tool 

OpenSUSE

	sudo zypper install gnome-tweak-tool 

Now you are going to have to get some icons/themes/cursors. You can bassiclu get the cursors and icons from anywhere, but you need to get the GTK themes from gnome-look.org. You will need to make get them to show up. Make sure that in your home directory, that you create 2 directories. Make “.themes” and make sure that all of your GTK themes go here. Then, create a directory called “.icons” and make sure that you put your icons packs and cursors here. Now, simply go into gnome-tweak-tool and change your icon and cursor theme. 

You may notice, that even though you have put the GTK theme in the .themes folder, you can’t switch to it. This is where extensions come in. Extensions are thing that you add to the gnome shell from your browser. You can get them from “extentions.gnome.org”. To switch themes, simply search for “userthemes” and install the extensions. There are a bunch of extensions for basically everything that you could ever want. Make sure to play around with extensions. 

Now, you should have a better idea on how to customize the Gnome desktop environment. You should now be able to install extensions, change icons, change cursors, and change themes. Allowing your gnome desktop to truly be yours.
