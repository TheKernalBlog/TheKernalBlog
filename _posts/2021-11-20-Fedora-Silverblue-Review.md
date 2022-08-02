---
published: true
---
Nowadays it seems that many Linux distro's aren't doing any innovating. Most of them now are just rebuilds of an
existing Linux distro with a new desktop or default apps. However, the team at Fedora are known to innovate. One of 
their newest inventions is Fedora Silverblue. Silverblue is a very interesting OS that I have been trying 
out for about a week. I am going to give a general review of this amazing Linux distro, what is good about 
it, and what its problems are. 

# Stability 

Fedora Silverblue is one of the most stable operating systems ever created. This is because everyone that 
uses Fedora Silverblue uses the same base image. All of your applications are Flatpaks, so nothing should 
ever break, and if it does it should be fixed almost immediately. Nothing for me has ever broken at all. Even if it did, like OpenSUSE you can easily rollback to a previous image. 

# rpm-ostree 

If you tried out Fedora Silverblue, you would realize that unlike regular Fedora, DNF is not installed. There are two replacements, Flatpak and rpm-ostree. Fedora Silverblue is nothing but a base image with Flatpak, to update and change your image, you are going to use rpm-ostree. To update software, you just use, “rpm-ostree upgrade”. If you want to re-base to a different image, use “rpm-ostree rebase RELEASE”. If something doesn’t work on your new image, you can rollback using, “rpm-ostree rollback RELEASE”. Finally, if there is software that you would like to install or uninstall you can do so with “rpm-ostree install” and “rpm-ostree uninstall”. 

# Flatpak 

Due to the fact that you don’t want to install applications on the actual system image, most of your applications are going to be installed as Flatpaks. While Flatpak’s are very close in concept to Snap packages, Flatpaks are not only completely open sourced, but they are just as fast as regular applications. Due to the fact that they are sandboxed, they are better for privacy as they can’t interact with the rest of the system. This means that they will not use the system theme by default though, but you can apply GTK themes using Flatseal. Flatpak also has almost every application under the sun, especially if you decide to add the Flathub repository. 

# Immutability 

Unlike most other Linux operating systems, the root file system for Silverblue is mounted as read-only by default. This makes the system even more stable, while making it more secure as well. You can’t get the system to a state where it is completely broken, so someone can’t just run a malicious executable and destroy your computer. 

# My Problems 

This is all great and all, but there are really some problems with this OS. One of the biggest problems is rpm-ostree. While it is the biggest pro of Silverblue, it is also the worst part. Rpm-ostree requires you to reboot every time that you update or install an application. This is a big problem if you care about uptime, so please don’t ever think of using Silverblue on a server. Silverblue also currently has only 2 desktop environments available, KDE and GNOME are your only options. There is work to be done for LXQT and i3, but they are not ready yet. 

# Conclusion 

Fedora Silverblue is something that I would check out if you would like to use something new. I truly believe that Silverblue is the future, and that with a few more options and some polish, it could be amazing.
