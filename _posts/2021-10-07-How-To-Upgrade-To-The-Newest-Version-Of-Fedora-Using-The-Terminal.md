---
published: true
---
One of the things that I and many other people like about Fedora is that it updates very regularly. Even though it has a point release schedule, it usually has the latest version of software. So it seems reasonable that you are going to want to upgrade to the next version whenever it is available. And with the release of Fedora 35 right around the corner, many users are going to want to upgrade. I am going to show you how you can ugrade to the next version of Fedora using the terminal. 

# Updating the current system 

Before you update, you are going to want to make sure that all of your packages are 100% up to date. This can be achieved using this one command. 

	sudo dnf -y update

# Installing the DNF plugin 

DNF will not allow you to upgrade to the next version without installing the system plugin. You can copy-paste this command to install the system upgrade plugin. 

	sudo dnf install dnf-plugin-system-upgrade

# Download the next version 

Using the plugin that you just downloaded, you can download the next version using this command. 

	sudo dnf system-upgrade download –releasever=INSERT NUMBER 

You are going to want to insert the number of the version that you would like to download. As an example, this is how it would look if you were upgrading to version number 34.

	sudo dnf system-upgrade download –releasever=34 

# Rebooting into the newest version 

To finish the system upgrade, you are going to have to put this in your terminal. 

	sudo dnf system-upgrade reboot

# Conclusion 

When you reboot, you should find that you are using the newest version of Fedora. Make sure to follow the Fedora team to find out when the newest version of Fedora is coming out, then use the simple command line tool to get all of the newest bells and whistles.
