---
published: true
---
Suckless is one of the best and most popular non-GNU software projects for Linux & Unix like operating systems. They have made some of the fastest and best apps available right now, such as dwm, st, dmenu, and surf. While the software is useful, it can be a little hard to install properly, as it requires building from source. But no worries, I am here to show you how to correctly obtain all of the dependencies, get the code, and build it.

# Installing Dependencies

If you just try to build the software from source on Debian or Fedora, you will realize that you get a lot of errors. This is most likely caused by missing dependencies
. You can install them with this command.

## Debian/Ubuntu

        sudo apt install make gcc libx11-dev libxft-dev libxinerama-dev xorg

## Fedora/CentOS

        sudo dnf install libX11-devel libXft-devel libXinerama-devel make gcc xorg

# Cloning The Software

For the purpouses of this guide, I am going to use git. If you don't have git, you can just install it with your package manager like so.

## Debian

        sudo apt install git

## Fedora/CentOS

        sudo dnf install git

## Arch/Artix

        sudo pacman -S git

Then, you can use git to clone the software of your choice with these commands. I personally have a "Suckless" directory in /home/, where I clone these direcrory's.

## dwm

        git clone https://git.suckless.org/dwm

## st

        git clone https://git.suckless.org/st

## dmenu

        git clone https://git.suckless.org/dmenu

## Surf

        git clone https://git.suckless.org/surf

# Building the software

You're almost there, you just have to use make to build the software from source. Don't worry, it won't take long. Just go into the directory and run this command.

        sudo make clean install

# You're Done!

You have succesfully cloned and built whatever suckless software you needed. While it may seem like a hassle to go through all of this work instead of just using the package manager, building from source will open up a new world of options for configuring your software., until eventually you can start applying patches to the source co
de and recompiling.
