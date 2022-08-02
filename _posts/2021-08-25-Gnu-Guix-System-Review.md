---
published: true
---
NixOS is an incredibly popular Linux distro. The fact that it is rolling release and allows you to roll back to previous versions of packages makes it great for the power user. However, there is a competitor on the block. That is the “Gnu Guix System”. It is a Linux distro that uses the Guix package manager, the Linux-Libre Kernel, and the Shepherd Init system. After using it for a few days, I am going to go over the things that make this distro special, and why you might want to consider using it. 

# Guix Package Manager

The Guix Package manager is based on the Nix package manager. This means that you will be able to roll back to previous versions of packages like you would with Nix. The Guix package manager only has 100% fully free software. However, you can use the <a href="https://gitlab.com/nonguix/nonguix">Non guix</a>  repository to get some nonfree software that you wouldn’t be able to get otherwise. It is rolling release, meaning that you are going to be able to get the newest versions of software. It is also worth noting that you can install Gnu Guix as a package manager on top of a lot of distros. 

# Linux-Libre Kernel 

The Linux-Libre Kernel is a modified version of the Linux kernel that does not include any nonfree licenses or binary blobs. This allows you to be sure that there is no proprietary code in your operating system. However, the Linux-Libre kernel will not work with a lot of machines due to the fact that it does not have any of the binary blobs that make Wifi work on many other distros. No need to panic though, as you can get the regular flagship Linux kernel too. I would prefer that they include a iso with the regular Linux kernel, but installation with the regular Linux kernel is not hard at all. 

# Shepherd init system 

Systemd has been getting a lot of hate for being too slow. Luckily for any Systemd haters, Gnu Guix uses the Shepherd init system. It is a fairly easy to use and super fast init system. For example, if you would like to start a service all you have to do in enable it, and then set it to start like so. I am using the LX Display manager as a example. 

	herd enable lxdm

	herd start lxdm 

You can also remove it easily using the “herd stop” command. Again, using the LX Display manager as a example. 

	Herd stop lxdm

If you would like to learn more about the init system, the Gnu project has their own documentation <a href="https://www.gnu.org/software/shepherd">Here</a> 

# Conclusion 

Gnu Guix System is a very unusual Linux distro. The 100% free approach it takes and the unusual init system may put some people off. However, if you are in the market for a rolling release, super fast, and 100% free Linux distro I would recommend that you check the Gnu Guix System out. 

If you would like to see their official page, you can click the link below. 

<a href="https://guix.gnu.org/">Click Me!</a>
