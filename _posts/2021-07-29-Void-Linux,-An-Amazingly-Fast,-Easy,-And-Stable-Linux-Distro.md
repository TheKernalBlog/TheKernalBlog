---
published: true
---
Here is the thing. I love Qubes. It is amazing for privacy, separating my workspaces, and being secure. However, I wanted to play some games. The problem is that Qubes runs everything in a VM without even accessing the GPU. So, I needed a good Linux distro, and I settled on Void with musl. So, I am going to explain why you might want to consider using Void Linux. 

## Installation 

The installation is very easy, despite not being GUI. It has a CLI installer that you can aces by typing “void-installer”  in the terminal. As long as you know how to use Cfdisk to make partitions, you should be completely fine. They even have a wiki page to help you out. 

## Desktop 

They have a lot of iso images downloadable. I prefer i3, so I took the regular image without a desktop. However, there is a option to install with enlightenment, Cinnamon, LXDE, LXQT, Mate, or XFCE desktops. You can also install and remove desktop environments easily after the installation. 

## Package Manager

Void Linux uses the xbps package manager. It is very easy to use, and is quite fast. You will ceritnly feel at home if you are a user of Pacman, as it is quite simaler. It is stable, so you will get some old packages, but not as stable as something like Debian or Rocky Linux. It is overall very great as a stable easy to use package manager.

## No Systemd

Void Linux does not use Systemd. While Systemd has it’s pro’s it is mostly just bloat. It has become more than just a innit system, meaning that there is just a lot of stuff that is not really needed. By not using Systemd, Void makes the boot time a whole lot faster. 

## Musl

Void Linux allows you to use Musl instead of Glibc. It is a option when downloading the iso’s. Musl is fast and small. It is faster, and a lot smaller. While there are cases where I would say it is better to use GlibC, Musl is great for anyone who needs the best performance possible. Plus, you can correct people when they say, “It’s GNU/Linux not Linux”, so that’s always fun. 

# Conclusion 

Void is great. It is super fast, and the option to use Musl makes it even faster. It is a great choice for desktops, and servers. It is rolling release, stable, and super fast. There is no distro that is just like it. Feel free to check it out in a VM, or just install it on your system. 



Here is the Wiki for the installation. (Unclickable For Your Security) 

https://docs.voidlinux.org/installation/live-images/guide.html
