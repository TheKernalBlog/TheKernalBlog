---
published: true
---
I am personally one of the people who likes to use a standalone window manager. Unlike many desktop environments, when using a standalone window manager like Openbox, i3, or BSPWM, there is no tool to configure the monitors on your own that comes pre-installed. Arandr is a Gui tool for the display configuration tool Xrandr. I am going to show you how you can install and use Arandr to configure your monitors. 

# Installing Arandr 

Depending on your Linux distro, copy-paste one of these commands into your terminal. 

Debian/Ubuntu based:

	sudo apt install arandr

# Arch based

	sudo pacman -S arandr

# Fedora/CentOS based:

	sudo dnf install arandr

# OpenSUSE

	sudo zypper in arandr

# Use and save Arandr configuration 

Launch Arandr, and then configure your monitors. Change primary monitors,  which monitors are on, where they are, and whatever else you need to do. Then click on “Layout”, and “Save As”. This will automatically prompt you to save in the “.screenlayout” directory. Pick the name as what you would like to save it as. I would recommend naming it something related to your monitor setup just in case you want to move monitors around but still keep the configuration. 

# Make executable 

So you have the script in the right place, but that won’t matter if you can’t run it. Simply run this in your terminal. 

	chmod +x ~/.screenlayout/NAME.sh

# Set to auto run

Finally, you need to set the script to autorun every time that you start up your window manager. In my case, using i3, I put this line into my ~/.config/i3/config file to start it. 

	exec_always –no-startup-id ~/.screenlayout/NAME.sh

And if you use Openbox, you would just have to put this into your ~/.config/openbox/autostart file. 

	~/.screenlayout/NAME.sh &

# You’re Done! 

If you have followed this guide, you now know how you can install Arandr, save the configuration, make it executable, and run it. You can have your monitors set up how you need without having to use a bloated desktop environment. If you would like to read up more on Arandr, click the link below. 

[Click Me!](https://christian.amsuess.com/tools/arandr/)
