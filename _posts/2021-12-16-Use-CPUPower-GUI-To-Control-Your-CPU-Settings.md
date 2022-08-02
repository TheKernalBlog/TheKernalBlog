---
published: true
---
Whether you are on a long trip and would like to conserve power, or you love playing video games and would like to boost your performance, it is good to have more control over your CPU. If you use GNOME, you will be familiar with the new performance settings in the panel, but there it does not provide the most control. If you would like to be able to easily tweak your CPU to the very last core, cpupower-gui is an amazing graphical utility for managing your CPU. I am going to show you how to install it, and how you can use it to configure your CPU settings. 


 # Instillation 
 
 The recommended way to install cpupower-gui on non Arch based systems is by using the OBS (Open Build Servive). The link can be found here, [[Click Me!]](https://software.opensuse.org/package/cpupower-gui?search_term=cpupower-gui). If you are using a RHEL or Debian based distro, download and then follow these steps. 
 
### Debian/Ubuntu
	sudo apt install ./PATH/TO/File.deb

### RHEL/Fedora/CentOS
	sudo dnf install ./PATH/TO/File.rpm

### Arch Linux

If you are using Arch Linux, you are in luck because like many other packages, cpupower-gui is in the AUR. Simply install it with this command, being sure to switch out yay with a different AUR helper of your choice. 

	yay -S cpupower-gui

# Usage 

## Preferences 
Once it is installed, you are ready to start. If you don't want to do any configuration yourself, you will notice a box called, "Profile". You can choose between battery saving, balanced, or performance.

## Profiles 
Here is where you can make different profiles for different use cases. For example, you can make a different profile for, "Gaming", "Compiling", "Browsing", etc. , 

## Settings 

This is where the real meat of the program is. Here is where you actually do all of the tweaking. You will be able to select any of the profiles that you have created, and can start the process of changing your CPU settings. You will see all of your CPU cores in a list, and you can change the minimum and maximum frequency settings, along with changing the governor policy and the energy preference. 

# Conclusion 

Cpupower-gui is a super useful tool that can benefit you in every situation. For me, playing video game, compiling software, and writing without a power cord are all made easier and more efficient with Cpupower-gui, I am sure that it will do the same for you. Go ahead and install it.
