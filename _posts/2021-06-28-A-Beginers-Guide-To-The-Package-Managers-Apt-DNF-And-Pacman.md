---
published: true
---

What is the best thing about Linux? Most people would say a package manager. They allow you to remove and install whatever software you want. In this guide, I am going to try to help absolute beginners wrap their heads around package managers. I am going to go over how to use the three most common package managers.

There are 3 main package managers on the linux world. There is apt, DNF, and Pacman. These were made for their respective distributions. Apt was made for Debain, Pacman was made for Arch, and DNF was made for red hat. I am going to break this blog into 3 parts. One for apt, one for Pacman, and one for DNF.

Apt:

Apt is the package manager that was designed for debian. It is what most beginers withh be use, because it is also the package manager for Ubuntu. Apt doesn’t have the newest software, but it is really easy to use.

If you want to install a package with Apt, type this.

Sudo apt install “package name”

If you want to update your packages, type this.

Sudo apt-get update

If you want to upgrade all of your software, type this.

Sudo apt-get upgrade

To remove software, type this.

Sudo apt remove “package name”

If you want to install using a .deb file, you can use apt to do this as well. Simply type this.

Sudo apt install /path/to/package.deb

DNF:

DNF is the package manager that was made for red hat. It is also the package manager for Fedora, and CentOS. It is a nice bridge between being stable, and having some of the newest software. Being the package manager for Fedora makes it really popular.

If you want to install a package with DNF, type this.

Sudo dnf install “package name”

If you want to update your packages while upgrading your software, type this.

Sudo dnf update

If you want to remove software type this

sudo dnf remove “package name”

Finally, If you would like to install using a .rpm file, you can simple do the same thing you ould do with a .deb file and apt. Type this.

Sudo dnf install /path/to/software.rpm

Finally, the last package manager that I am going to cover is pacman. Pacman is the package manager for arch. If you installed arch, you probably don’t need this guide. However, Manjaro has Pacman while still being really easy for beginners.
To install software using pacman, type this.

Sudo pacman -S “Package name”

To update the pacman database and software, type this.

Sudo pacman -Syy

To remove software using pacman, type this.

Sudo pacman -R “package name”

If you are new to using linux, these commands are all that you need to update, install, and remove all of the software that you need. Package managers can be hard to learn, but it is the fastest, most efficient, and easiest way to install anything on linux.
