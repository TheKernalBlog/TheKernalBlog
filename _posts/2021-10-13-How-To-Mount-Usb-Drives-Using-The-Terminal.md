---
published: true
---
If you are reading this, there is a good chance that you are running a minimal Linux distro like Arch, Void, or another distro that only comes with a TTY. This means that in most cases, when you put in a USB drive, it won’t mount onto the system. I recently had to do this, so I am going to show you how to manually find the usb drive on your system and mount it. 

# Find the name of the USB 

First plug the USB in. The best way to find the name of the USB, is to run the lsblk command. It should be pretty easy to find out which one is your hard drive, because it should have the root partition along with the EFI partition. Simply run this command to find the name.

	lsblk -p | grep "disk\|part"

In my case, the USB is named /dev/sdb, however this may not be the same for you. 

# Create the mount point 

You are going to make a directory in the /mnt/ directory. This can be anything, however for the purposes of the demonstration I am going to name it “usb”. Simply copy-paste this command in the terminal. 

	sudo mkdir -p /mtn/usb 

# Mount the USB

Now that the mount point is created, mounting the USB is super easy. Simply type the mount command, followed by the name of the USB and the mountpoint. Using the previous examples, this is what you would have to do to mount the USB. 

	sudo mount /dev/sdb /mtn/usb

# You’re Done!

You should now be able to access the contents of the USB drive. This is super helpful if you are going to be flashing any other systems with Linux, or if you have a lot of files that are stored in a USB.
