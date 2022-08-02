---
published: true
---
Has it ever happened to you where maybe you were updating and it broke the system, or that you have done something stupid and broken your system? I know that feeling all too well. However, as long as you have a working GUI you are able to revert to a backup of your system using timeshift. I am going to explain how you can install and backup your system using the timeshift utility on Debian and Ubuntu based Linux distro’s. 

# Instillation 

Instillaiton on is very simple. Simply copy-paste these commands in your terminal depending on what Linux distro that you use. 

# Ubuntu/Debian
	sudo apt install timeshift

# Fedora 
	sudo dnf install timeshift

# Arch
## Assuming that you have the yay AUR helper
	yay -S timeshift 

# Selecting Snapshot Type 

If you are thinking, “I use ext4, this won’t work” you are mistaken. Due to RSYNC, you can create snapshots without having to use the BRFTS filesystem, however if you are using BRFTS there is also a selection to use that as well. 

# Creating the backup

Using the GUI, you can easilly click ‘create’ to make a backup of the file system. This may take about 5 or so minutes, depending on if you are using RCYNC or BRFTS. 

# Restoring the filesystem 

If you feel like you need to restore the file system, all you would need to do is open ‘restore’ and select the filesystems that you would like to restore. You can restore the root filesystem, boot filesystem, and home filesystem. This way if you have some files you need on your home filesystem, you can roll back without loosing all of your personal files. 

# Setting a schedule

It would be a bit stupid to have timeshift in case your system fails, and never do it regularly. So unless you are going to open up the application and save every day, it is a good idea to schedule it so happen every day or week. simply click on ‘Schedule’ in settings and you can set it up to backup every hour, month, week, daily, or whenever you boot. 

# Conclusion 

As someone who used to use OpenSUSE, the backup feature was one of the best things about it. Now with timeshift, knowing that you can do simmaler backups with any Linux distro and filesystem is so comforting, because as long as you keep backing up, your system can’t break unless you mess with the X server or boot loader.
