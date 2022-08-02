---
published: true
---
The Guix package manager is a higly reproducable and stable package manager based on the Nix package manager. It wan made by the FSF, meaning that it allows you to install a variety of 100% free software. The reproducability and saftey that comes with the Gnu Guix package manager is unrivaled. You may be tempted to install the “Gnu Guix System”, however you can instal the Gnu Guix package manager on any existing Gnu/Linux system. I am going to show you how you can install and use the Guix package manager. 

# Installation 

The FSF was kind enough to provide a isntaller script that will work on almost every Linux distro. It makes the install super easy. To start, login as root. 

	su – root

Now you are going to want to cd into the temporary directory to download the script. 

	cd /tmp 

Use the “wget” command to downlaod the script. 

	wget https://git.savannah.gnu.org/cgit/guix.git/plain/etc/guix-install.sh

Make the script executable with the chmod command. 

	chmod +x guix-install.sh

Then finally, run the script! 

	./guix-install.sh

After some waiting, you should finally have the Guix package manager installed on your system. Now all that you need to do is actually use it. 

# Usage 

 Unsuprisingly, you can install software with the “install” command. For example, 

	sudo guix install PACKAGE

You can then remove the software with the “remove” command. Like this. 

	sudo guix remove PACKAGE

Then you can upgrade all of your software with the “Upgrade” command like this   .

	sudo guix upgrade 

Lets say that a upgrade broke your software, or you removed something that you didn’t want to remove, you can essentially “time travel” by using the rollback command like so. 

	sudo guix PACKAGE –-roll-back 

# Conclusion 

You should now be able to install and use the Guix package manager on your non Guix systems. Allowing you to make use of the stable, rolling release, and 100% free package manager on any Linux distro that you would like. 

If you would like to check out their offfical website, you can click <a href="https://guix.gnu.org/">Right Here.</a>
