---
published: true
---
Using Arch Linux, there are many benifits. The fast speed, the amazing package manager, but one of the most cited reasons for using Arch is the AUR. The AUR is a repo that is maintained by the community, that anyone can add to. It has a lot of software that you can’t get using Pacman. However, there is no AUR helper on a default installation of Arch. The most popular is “yay”. I am going to explain how you can install, and use the yay AUR helper on a default installation of Arch Linux. 

# Getting ready to install 

For the installation you are going to need git. To do this you are also going to have to install the “base-devel” package. Just run these commands to get both of these. 

	sudo pacman -S base-devel 

	sudo pacman -S git 

# Installing 

When installing something without a package manager or AUR helper, it is safer to go to /opt. Cd into the directory using this command. 

	cd /opt 

Then you use git to clone the “yay” directory. Copy/paste this command. 

	
	sudo git clone https://aur.archlinux.org/yay.git
You now have to change the ownership of this file. You can do this by running this command, making sure that you add your username. 

	sudo chown -R USERNAME ./yay 

All that there is to do now is to build yay. Run these two commands to cd into the direcotry and build it. 

Going to the direcotry: 

	cd yay 

Compiling it: 

	makepkg -si 

# Usage 

Now That you have installed, you are going to have to learn how to use it. It is very simmaler to pacman. Here are some of the commands you need to learn if you want to use yay. 

Updating: 

	yay -Syu

Installing packages: 

	yay -S PACKAGENAME

Removing packages: 

	yay -R PACKAGENAME

# Conclusion 

Now you are able to install, and use the yay AUR helper on Arch Linux. You will have easy, and fast acces to any of the thousands of packages on the AUR. Making it so that you can install bassicly anything that you could ever need without fear of worrying that it is not in the repo’s.
