---
published: true
---
Everyone is super excited about the new stable release of Debian. Debian Bullseye has been  a huge success and has made Debian a significantly more usable and and Fast Linux distro. However, one version of Debian that often gets overlooked is “Sid”. Sid is the rolling release version of Debian, that allows you to get the absolute newest version of software, drivers, and kernels. If you would like to use this amazing version of Debian, I am going to show you how you can convert Debian “Stable” to Sid.

# Editing The Apt Sources File 

Unlike Debian stable, Sid doesn’t have a iso that you can download. You are going to have to take a existing Debian install and turn it into Sid. You can do this by editing the “/etc/apt/sources.list” file. Open it up with your favorite text editor, making sure that you open it with root. There should be three lines of code. If you are using Debian 11 to follow this guide, your sources.list file should look like this without any changes. 

	deb http://deb.debian.org/debian bullseye main 

	deb-src http://deb.debian.org/debian bullseye main

	deb http://deb.debian.org/debian bullseye-updates main

	deb-src http://deb.debian.org/debian bullseye-updates main

	deb http://security.debian.org/debian-security/ bullseye-security main

	deb-src http://security.debian.org/debian-security/ bullseye-security main

You are going to want to delete/comment out all of the lines instead of the first two. While you may think that deleting the security and updates repo may harm the system’s security, there is no reason to worry. After converting to Sid, you won’t have to worry about security updates because you will receive the latest software anyways. 

Now you have to replace the “bullseye” in the first two lines with “sid”. After doing these two things, your sources.list file should look like this. 

deb http://deb.debian.org/debian sid main

deb-src http://deb.debian.org/debian sid main

# Converting to Debian Sid 

Before you do the “dist-upgrade” command you are going to have to update the new repositories. Simply using this command. 

	sudo apt-get update

Then you are going to run the dist-upgrade command. Don’t be alarmed if this takes quite a while, as you are updating a whole lot of packages. Just copy-paste this into your terminal. 

	sudo apt-get dist-upgrade 

Now after your upgrade, there are going to be some packages that are no longer needed. Use the autoremove command to get rid of them. 

	Sudo apt-get autoremove 

Finally, you can reboot. Once you do, you will be using Debian Sid. 

# Conclusion 

If you have followed all of the instructions, you should now be able to use Debian Sid. While the upgrade process is not very simple, I would say that it is 100% worth it. Having a rolling release Debian is great for personal computers and servers that need the newest version of packages.

If you would like to see more information about Debian Sid on the offical Debian Wiki, you can click the link below. 

<a href="https://wiki.debian.org/DebianUnstable">Click Me!</a>
