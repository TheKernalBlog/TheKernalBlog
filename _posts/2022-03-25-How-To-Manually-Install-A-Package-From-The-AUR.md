---
published: true
---
The AUR is one of the best ideas anyone has had when it comes to desktop Linux, and it has undoubtedly allowed Arch to grow into the incredibly popular and mature distro that it is now. Yet, many people only really use it to install one or two programs. So, if you are one of those people, and can't justify having a AUR helper, I am going to show you how to setup, clone, and install an AUR package manually.

## Installing The Dependencies

Aside from a few developer packages, all of the dependencies for actually building the software is actually already installed. But, if you are going to get the PKGBUILD, you need to use git. So, if you haven't already, just install it with this command.

        sudo pacman -S --needed base-devel git

## Grabbing the PKGBUILD from the AUR.

In order to get the PKGBUILD, you need to go to the AUR section of the Arch Linux website. From there, you can search for the package that you would like to install, and then grab the git clone URL. Then, clone it using this command.

        git clone https://aur.archlinux.org/PACKAGE.git

## Installing the package

Now it is time to install your package. To start of, cd into the directory of the PKGBUILD you just cloned.

        cd DIRECTORY NAME

Then, you can just run this command to install your newly cloned PKGBUILD.

        makepkg -si

It will start compiling, and then ask for your password. Itmay take a while, so just feel free to let it run in the background while you do other things.

# You're Done!!!

You have now installed a package from the AUR, without having to deal with all of the Spaghetti code that comes with using a AUR helper. I would not recommend doing this if you install a bunch of packages from the AUR, but if you install just a few packages and don't mind doing this every time that you need to update, this is a great choice for you. Sometimes it is just better to do things the ol' fashioned way.


~
~
~
