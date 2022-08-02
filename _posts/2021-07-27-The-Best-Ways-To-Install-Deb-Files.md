---
published: true
---
When software is not in the repo’s, You will have to use other options. Snap, Flatpak, and appimages are all good. However, when using Debian/Ubuntu based distros there is a option that in my opinion is better than all of these. Deb files. Deb files are files that allow you to install the package on your system using a file. Most applications will have their .deb file online. However, they can be difficult to install. I am going to go over the best way to use .deb files to install software on your system. 


# Gdebi 


## Installing Gdebi

While the other options are installed on every Debian based distro, there is a chance that you may have to install Gdebi depending on what distro you use. It is pre-installed on Ubuntu and Debian. To install it, simply type this in your terminal. 

	sudo apt-get install gdebi

## Graphical Install using Gdebi

Now that you have Gdebi installed there are two ways to use it. Graphically, or using the terminal. To use it graphically, open your file manager and go to where your .deb file is. Right click on the .deb file. Click on the “open with” option and choose Gdebi. Your .deb fie will now start installing. 

## Terminal Install Using Gdebi 

There are some people who love to use the terminal for everything. Luckily, Gdebi allows you to use it in the terminal  too. Simply Cd into the directory where the .deb file is, and type this command. 

	sudo gedbi NameOfFile.deb

This will do functionally the same thing as using Gdebi graphically, but it is super convenient if you just want to install it like you would any other apt package. Speaking of apt packages. 

# Apt

Using apt is my preferred way of installing .deb files. It is not graphical, but is is very easy and means that you not only don’t have to install anything, but you don’t have to fix anything after the installation either. To install using apt, you will have to use the terminal to cd into the directory where the .deb file is. Then type this in the terminal. 

	sudo apt install ./NameOfFile.deb


# Dpkg 

I’m just going to be honest, I am not a fan of this method. It makes you fix the software after you install it, but I am going to tell you how to do it anyway, Much like apt, you are going to have to cd into the directory. Then you are going to have to type this command to install it. 
	Sudo dpkg -i NameOfFile.deb

Dpkg will often break the package by not installing the dependencies. You are going to have to fix it using apt. To  fix it, type this in the terminal. 

	sudo apt-get install -f


# Conclusion

These are all excellent ways of installing .deb files. If you want a graphical experience, I would recommend Gdebi. If you want to install it using the termal as a regular user, I would say that apt is the best option. However, dpkg still has it’s uses if you are trying to install something without the dependencies. I think that trying all of these out is the best option, to see witch one you like the most, as they are all different and have something they are good at.
