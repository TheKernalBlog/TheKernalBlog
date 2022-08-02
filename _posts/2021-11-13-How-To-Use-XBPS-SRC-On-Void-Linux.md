---
published: true
---
Void Linux is a increasingly popular Linux distribution. Because it is systemd-free, and offers 
a version with the musl libc, people are really starting to catch on. Another reason to consider 
using Void is the amazing package managment system. Xbps is one of the best package managers of
all time, and one of the reasons for that is xbps-src. I am going to explain to you what 
xbps-src is, how you can set xbps-src up, and how you can use it to install packages. 

# What is xbps-src

Before you can understand what xbps-src is, you are going to need to understand what it is not. 
It is not a seperate package manager, nor is it a plugin for the xbps package manager. Xbps-src
itself is nothing but a bash script that allows you to build source packages into binaries that 
you can use xbps to install. The main reason you would use it is to install packages that are not
in the offical repositories.


# Setting up xbps-src

First, make sure that you have git installed. Run this command in your terminal if it is not.

	sudo xbps-install git

Then you are going to need to clone the void-packages repo from github. Depending on your
internet speed, this may take a while. Use this command in the terminal. 

	git clone https://github.com/void-linux/void-packages.git

Then, cd into the newly created directory. 

	cd void-packages

Now, it is time to install the binary bootstrap. This is what will allow you to build these 
binaries in the first place. Use this command in the terminal. 

	./xbps-src binary-bootstrap

# Building packages 

For the perpouse of this explanation, I am going to install busybox-core, because I personally 
use busybox. This will work for any package though. Here would be what you would do to for the
instillation of busybox. 

	./xbps-src pkg busybox-core

It will now be available as in the binpkgs directory. 

# Installing the Binary packages 

You are going to have to use the regular xbps-install command to install the binary. Here would
be the command to install the newly created busybox binary. 

	xbps-install --repository void-packages/binpkgs busybox-core

# Conclusion 

You should now be able to build and install packages using xbps-src. This is a super usefull 
feature that I love. It really is one of the most amazing features of the Void linux distro. 
It really shows how inspired Void linux is by the BSD familly of distros. You should now be 
able to install and use packages using xbps-src.
