---
published: true
---
Even though some people don't like it, Bluetooth is very big right now. From headphones, mice, keyboards, and speakers using Bluetooth by the day it is a good idea to have Bluetooth available on your Linux machine. So if you don't have Bluetooth on your distro, or if you are installing a minimal distro, I will show you how to install and setup Bluetooth with your GUI. 

# Installing the essentials 

To get bluetooth working with a GUI you are going to need to install bluez, and blueman. Depending on your Linux distro, copy-paste these commands in the terminal. 

## Arch
	sudo pacman -S bluez bluez-utils blueman 

## Debian/Ubuntu 
	sudo apt install bluez bluez-utils blueman 

## RHEL/CentOS/Fedora
	sudo dnf install bluez bluez-utils blueman 

## SUSE/OpenSUSE 
	sudo zypper install bluez bluez-utils blueman 

# Enabling the service 

Assuming that you are using systemd, this is what you will have to do to start the bluetooth service or enabling it to start at boot. 

## Starting 
	sudo systemctl start bluetooth.service 

## Starting at boot 
	sudo systemctl enable bluetooth.service 

# Conclusion 

You can now make use of bluetooth technology on your Linux machine. Whether you are installing the headless version of a OS so that you can install a window manager, or you are looking to add bluetooth to your server, using bluez and blueman makes pairing and using bluetooth devices easy.
