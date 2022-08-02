---
published: true
---
Arch is a great distro. It has amazing community support, it is fast, and cutting edge. The AUR and the speed of Pacman make it one of the best distros arround. However, it can be difficult to install. It doesn’t come with any desktop, or easy wifi usage. There is a solution though. Archbang! Archbang is bassicly arch with Openbox, a few packages, and most importantly, an installer. I am going to go over how to install Archbang onto your system, so that you can have the full Arch experience without actually having to install it. 

# Starting the installer 

By right  clicking on the desktop, you should see the option to load the installer. However, if you don’t have that option you can load up a terminal and type “abinstall”. This will load the installer. 

# Making The Partitions 

After booting up the installer, you should see a cli installer with a bunch of choices. The first one is prompting you to make partitions. So, you will need to type the letter “1” to begin the process. 	You will be asked what you want to use to create the partitions. I would choose Cfdisk, because I find it easiest to use. You will create 3 paritions. One that is half the size of your ram that will be used as swap, One 500mb that will be used as the efi partition, and one taking up the rest of the hard drive that will be used for root. Write the changes, and back out. You will be asked what partitions should be used for what, make sure that you choose the correct partitions. When asked if you want to use for the home partition, choose for there to be no home partition. Then, you will be done and be thrust back to the main installer screen. 

# Installing

Now that the hard part is done, you can actually install it. Type ”2” to start the installer. This is the most simple part of the install because all that you have to do is wait. Once it is done, just go back to the main install screen. 

# Hostname
You may think that just because you have installed it you are done. Nope. You still have to do much more. You will have to pick the name of your computer. In the main installer menu, type “3” and you will be able to choose the hostname for your system. The default is “archbang”, but I prefer to change it. Once you pick the hostname, you will be kicked back to the installer menu. 

# Location

You are going to have to pick your location. This is pretty standard. Simply type “4” and you will be able to get into the location chooser. You will see a list that has a bunch of regions. Just pick yours and you can move on to the next step in the install process. 

# Hardware Clock

This is where you are going to choose between UTC or local time. It doesn’t matter much. I personally like UTC. Type “5”, and then choose whatever you want for your hardware clock. Then you will be booted back to the main installer menu. 

# Locale 

You are going to have to pick your language. This will be used in in the console. Type “6” in the main menu. You will pick the language that you are most comforitable with. Then go back to the main menu. 

# Desktop Keyboard Layout

You are going to have to pick your keyboard layout. Make sure that you know what keyboard you have. Type “7” on the main installer menu, choose your keyboard. In my case EN_US, then you will be put back to the main installer menu again. 

# Bootloader

Now it is time to pick your bootloader. You have 3 options, Grub2, Systemd-boot, and Syslinux. I personally like Systemd-boot, however I would recommend Grub2 to most people. Once you have choosen, back out to the main menu. 

# Root Password 

This is one of the most important steps. This will be what allows you to do anything that requires root. Type “9” in the main menu, and then pick a strong password that you will not forget. 

# Making The User Account 

You are finally on the last step of the install. Type “10” in the main menu to create your user. You will pick your username, and your password. This is what you will use to login. Once you are done with this step, you can close the installer, and reboot. 

# Fixing Pacman After The Install 

For some reason, the keys are all aut of wack after the install. To fix them, you will have to imput these three commands to get pacman up and running. 

	sudo pacman-key -init

	sudo pacman -key -populate archlinux 

	sudo pacman -Syyu archlinux-keyring

# Conclusion

If you have followed all of these steps, you should have a fully working Archbang install. I always prefer this to installing Arch normally, and it is a lot easier for any newcomers to linux.
