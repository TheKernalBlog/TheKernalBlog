---
published: true
---
When using Red Hat based distros like Rocky, CentOS, or Fedora one of the main complaints is that the package manager, “dnf” is slow. I would actually agree with that opinion. The default dnf package manager without any configuration is quite a bit slower than many other package managers like apt, pacman, or nix. However, there are a few ways that you can make it a lot faster. I am going to showcase two ways, the manual way by editing the dnf config file, or by downloading and running a script called ‘Dnf-Fast”. 

# Editing the config file. 

You are going to need to open up the /etc/dnf/dnf.conf file with super user privileges using your favorite text editor. In my case, that is nano. 

	sudo nano /etc/dnf/dnf.conf

Then, copy-paste these two lines into there. This will not only insure that you have the fastest download mirror, but it will allow you to download more packages at a time. 

	fastestmirror=true 

	max_parallel_downloads=10

Then, you are done! This personally is what I do, and it has speed up dnf a lot. 

# Downloading DNF-Faster

Before you do anything, you are going to need to install 3 packages to make this work. Aria2, patch, and git. Simply install them using this command. 

	sudo dnf install git aria2 patch

Then you need to clone the git repository. Just copy-paste this command in your terminal. 

	git clone https://github.com/chitholian/DNF-Faster.git

Cd into the newly cloned directory. 

	cd DNF-Faster

Then, finally, you can use the “patch” command like so. 

	sudo patch -p0 -d/ -b < dnf-faster.patch

Now DNF will use aria2 to download all of it’s packages using what is called “parallel multiconnection”. This is also what the more popular “apt-fast” does to speed up apt. 

If you would like to check out the github for DNF-Faster yourself, click on the link below. 

[Click Me!](https://github.com/chitholian/DNF-Faster)

# Conclusion 


Both of these methods will allow you to install and update packages at very high speeds, making your life a lot easier especially if you are using Fedora and have to update a lot. While DNF is already a lot faster than “yum” you can now enjoy the beauty of RHEL based distros while having the download time of other distros.
