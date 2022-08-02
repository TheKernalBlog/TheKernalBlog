---
published: true
---
When you use OpenSUSE, you have quite a few packages available to you. When you factor in the OBS, you have almost every package under the sun. However, it is always great to have a few extra packages in your repositories, W\which is why the Packman repository exists. If you use OpenSUSE Leap or Tumbleweed, Packman is a must, and I am going to show you how you can install the repository. 

# Using a GUI

Thanks to the amazing system management software that is YaST, you can easily add the repository using a graphical interface. Open “YaST Software Repositories”, and click on “Add”. Once you click on “Add” select “Community Repositories”, then click next. From there, you will be able to select between a few repositories. For the purposes of this guide, click on “Packman”. It will start the process of installing the repository. If you are asked to import any keys, import them and keep waiting for it to finish. 

# Using the Terminal 

If you are using OpenSUSE Tumbleweed, you can add packman by copy-pasting this command in your preferred terminal emulator. 

## Tumbleweed
	sudo zypper ar -cfp 90 https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/ packman

## Leap

If you prefer a more stable experience, but still want all of the necessities that Packman provides, simply copy-paste this command into your terminal. 

	sudo zypper ar -cfp 90 'https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Leap_$releasever/' packman

# Using Packman 

You may realize that if you do an upgrade with the new Packman repository, it will list a bunch of applications that will not be updated. In order to upgrade them, use this command in the terminal, changing the vendor from the regular repositories to Packman. 

	sudo zypper dup --from packman-essentials --allow-vendor-change 

# Conclusion 

You have now added the Packman repository to either your OpenSUSE Leap or Tumbleweed installation. This will give you the freedom to install and use a bunch of applications, expanding your package pool from just the regular repositories and the OBS, to being able to install almost anything you could ever need. Because it is always better to have more available to you.
