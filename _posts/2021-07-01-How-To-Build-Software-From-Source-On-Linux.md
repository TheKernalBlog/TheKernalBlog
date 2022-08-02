---
published: true
---

For most Linux Distro’s, you have a large amount of software available to you from the package manager. However, sometimes it is not in the package manager, or available as a appimage. What do you do now? You are going to have to build it from source. Taking the source code of the software and building it yourself has been around as long as Linux. So I am going to go over how to take the source code of software, and build it yourself. 

The first step is to actually get the source code. This can be done using the “git” command. This is often included in many distro’s, but you should be able to install it from your package manager of choice. Now you will need to go to the github page of the software that you want to build from source. Simply go to the “Downloads” button and copy the link. From there, you can type this in the terminal. 

$ Git clone “Link You Got From Github” 

Now you will see a file in your home directory. To install it, you will have to go to your terminal and type these commands. 

$ cd “Name Of File”

You will need to change to the directory of the file that you just cloned using git. 

$ ./configure 

This will get everything ready for the installation. Make sure that you don’t skip this step. 

$ make 

Now, you will finally have to install it. 

$ make install 

Congrats! You have just installed the software that you needed from source. This can be a great alternative or substitute for a package manager. With this, no software is going to be out of your reach. You can install anything.
