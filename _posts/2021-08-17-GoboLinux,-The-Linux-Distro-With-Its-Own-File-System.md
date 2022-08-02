---
published: true
---
When you use Linux, it is most likely that you are using either the Fat32, or Ext4 file system. They are almost exactly the same. However, there is a Linux Distro that has it’s own filesystem. Unlike most Linux distros, Gobo Linux takes a Mac-OS like approach to a file system. I am going to go over the file system, the desktop, and more. 

# The Filesystem 

The regular Linux filesystem can be quite confusing. With /etc, /bin, and /usr, you can sometimes have some trouble finding exactly what you want. GoboLinux decides to use just 5 directory’s for it’s main filesystem. I am going to go over how you can navigate this filesystem. 

## Programs 

While on a regular Linux distro your applications are spread out all over the place, here every applications has it’s own file that includes it’s settings. Configurations, and data. Like NixOS, this allows you to install different versions of the same applications 		

## Users 

This contains the home folders of all of the users. This includes root, and any other users that you would wish to have during the install. 

## System 

This is where all of the files that the system needs to run are. The Bainaries and the Kernal are both placed here. 

## Data

This is where all of the information about all of the packages is placed. It also contains the folder for all of the variables. 

## Mount 

In a regular root file system on Linux, you can have a /mnt file for mounting  anything that may need mounting, like a SSD or USB. This is basically the exact same thing. 

# Packages 

GoboLinux takes a very Gentoo like approach to installing packages. It uses the “compile” command to grab the source code, and compile anything that you may need. However, due to the fact that it compiles everything from source, installing and updating packages will take a long time. 

# Installation 

So, you want to install it? Luckily for you, it comes with a live mode and a guided installer. After you boot the USB you will start in a command mode interface. However, you can get a desktop by starting xorg with the “startx” command. Then you can test it out using the awesome window manager. It comes with a guided installer that is very easy to use. I would’ve hoped for something like Calamares, but the installer that they use is very good at what it does. 

# Conclusion 

While I would not recommend it to long time Linux users who want a traditional unix-like filesystem, if you are in the mood for a Linux distro that simplifies the file system, and are fine with the long download times of compiling everything from source, I would 100% recommend that you try it out. It is a really unique distro that deserves all the love and praise that it gets.
