---
published: true
---
Ubuntu is a point release distro, meaning that it has multiple releases that you update between. However, there are many people who would instead prefer to have a rolling release distro, where there is one release that gets continually updated. While some people would move to another distro, like Debian Sid, or even Arch Linux, there is a way that you can turn Ubuntu Linux into a rolling release distro. The method that I am going to show you today, it a lot faster than doing it manually, and it entails downloading a shell script which will automatically change you to the 'devel' release. 

## Making sure that you are already updated on your version. 

Before running anything that will mess with your sources.list file, it is always recommended that you make sure that you are already up to date so that nothing goes wrong when you make the upgrade. You can use apt to update all of your software like so. 

	sudo apt update && sudo apt upgrade

## Installing git. 

The chances are, that if you have been using Ubuntu for a while, git is probably already installed, but if it isn't, you can install it like so. 

	sudo apt install git

## Cloning and running the script. 

You can download the script from git using this command. 

	git clone https://github.com/wimpysworld/rolling-rhino.git

This will put the 'rolling-rhino' directory into your home directory. Open it like so. 

	cd rolling-rhino 

Now, all that is left to do it run the script. Make sure that you run it with super user permissions or else it won't work. 

	sudo ./rolling-rhino

## Upgrading to rolling rhino and rebooting. 

When converting to a new release, you will have to use apt to do a distribution upgrade and then reboot, or you wasted all of your time following this guide. You can do the upgrade using this command. 

	sudo apt update && sudo apt dist-upgrade

Then, you can either reboot using the GUI or through the terminal like so. 

	sudo reboot

# You're done!!! 

You have now upgraded your Ubuntu machine to the 'devel', or 'developer' release. This means that on a daily basis you will get all of the new goodies and never have to upgrade to a new official release ever again. It is really nice to have all of the newest software, especially if you are a developer or a gamer that wants access to the latest games and drivers. This way, you can continue to use Ubuntu without having to deal with month-old software. 

