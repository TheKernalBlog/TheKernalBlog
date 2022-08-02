---
published: true
---
OpenSUSE. Much like CentOS or Fedora, it is the free and open sourced version of an enterprise Linux distro. In the case of OpenSUSE, it is based off of SUSE enterprise Linux. After playing around with it some, I have even switched to it from Void Linux. I am going to go over the reasons that you might want to use OpenSUSE, including the Software management, Yast, the different release models, installation,  and snapshots. 

# Software management 

OpenSUSE has a wide variety of software available. There are a few ways that you can install software. The first one is zypper, the package manager. It is a rpm based package manager that acts a lot like dnf. There is also the OpenSUSE Software store <a href="https://software.opensuse.org/">You can see here</a> . If you would like to use zypper with a graphical interface, you can also use the YaST software manager to install and use programs. 

# YaST

Yast stands for “Yet Another Setup tool”. It can be used as GUI tool, or can be run in a terminal with a TUI mode. It has almost anything that you could ever need. From managing services, changing software repo’s, to partitioning the disk. There is too much functionality to list. It is simple enough that a Linux newbie can use it to change simple things about the system, while someone with a lot of Linux experience can use it to it’s full potential. 

# Tumbleweed and Leap 

OpenSUSE has two different release models. Leap is more like the traditional “SUSE” distro in that it jumps from version to version. This is great for servers as you don’t have to update as often and it it more stable. I’ll say that from my personal experience, OpenSUSE Leap with snapshots is more stable than Debian Stable. There is even a server version for the Leap release model. OpenSUSE Tumbleweed follows a rolling release model that allows it to get cutting edge packages. This is what I would recommend for a regular desktop, as it allows you to make use of the newer software as soon as it comes out instead of waiting. The only real problem is that updates can take a lot of time, and stability is an issue. 

# Installation 

The installation of OpenSUSE is very straightforward. It is much like the old Debian installer. It’s all graphical and easy to navigate. Unless you are doing a dual boot, there is no need to partition anything. The live disk has options for Gnome, KDE, Or XFCE. I personally prefer to use the Netinstall option as you get more options on what you can install, including more desktop environments. The installation took around 30 minutes for me, but will be faster if you are using a SSD. 

# Snapshots 

This is one of the best reasons to use OpenSUSE for a server. Let’s say that something breaks after an update, you can easily go to YaST and  revert the file system to before the update took place. You can think about it like the Nix package managers “rollback”” function, but instead rolling back the entire file system. This one feature is the reason that OpenSUSE almost never breaks. 

# Conclusion 

There are many reasons why you would like to use OpenSUSE. If you want a rolling release RPM distro, if you want something super stable, or even if you just want something that is easy to install and maintain. OpenSUSE is a great Linux distro and I urge you to fire up a VM and try it out. 

If you would like to download it for yourself, feel free to click <a href="https://get.opensuse.org/">Here.</a>
