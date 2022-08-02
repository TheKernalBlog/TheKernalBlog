---
published: true
---
If you are coming from a Linux distro like Arch, you may notice that apt is a slow package manager in comparison. While apt itself is pretty slow, there has been some work done to make a faster version of the apt package manager. Apt-fast is a package manager that allows you to do simultanious downloads like you would with Arch, while you are still able to use the same repo’s. I am going to show you how you can install apt-fast. 

## Ubuntu 

The installation on Ubuntu is very straightforward. You simply have to install a download manager. I prefer Aria2, so that is what I am going to show you how to download. 

Install Aria2 with the following command.

	sudo apt-get install aria2 

Then you have to get the offical ppa. Just copy/paste this in your terminal. 

	sudo add-apt-repository ppa:apt-fast/stable

Then you need to update your repo’s. 

	sudo apt-get update

Finally, you can install the thing

	sudo apt-get install apt-fast 

## Debian 

Due to the fact that Debian does not use ppa’s, you are going to have to add this manually. Type these commands in your terminal. 

Install Aria2.

	sudo apt-get install aria2

Get the master direcotory. 

	wget https://github.com/ilikenwf/apt-fast/archive/master.zip

Unzip it. 

	wget https://github.com/ilikenwf/apt-fast/archive/master.zip

Cd into the directory. 

	cd apt-fast-master

Copy to user/bin 

	sudo cp apt-fast /usr/bin

Copy the config file too etc. 
	
	sudo cp apt-fast.conf /etc

Copy it to usr/share. 

	sudo cp ./man/apt-fast.8 /usr/share/man/man8

Use Gzip to uncompress it. 

	sudo gzip /usr/share/man/man8/apt-fast.8

Copy the config file to usr/share 

	sudo cp ./man/apt-fast.conf.5 /usr/share/man/man5

And finally, uncompress that. 

	sudo gzip /usr/share/man/man5/apt-fast.conf.5

# A Sidenote 

When you install it on Ubuntu, you are going to have to run through  installation page where you choose the max amount of downloads, and the repo’s. However, you can edit the config file at any time by editing /etc/apt-fast.conf. 

# Conclusion 

Now you have installed apt-fast. This means that your upgrade, and install times will be super fast. While the instllation can be a bit of a pain, it is 100% worth it because you will save hours on update time.
