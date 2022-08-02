---
published: true
---
Software for Linux is a lot more complicated than, say, software for MacOs. Instead of having one simple binary that you update for every version of the operating system, you have hundreds of binaries for many Linux distros, with different package managers, formats, init systems, and even userlands. Many people see this as an issue, and try to use a universal package manager, and then they fight about which universal package manager to use. But, I am here to propose, that not only is the fragmenting of Linux not an issue, universal package managers are unneeded and inefficient.

## Fragmentation is not an issue

In almost every discussion about universal package managers, it seems, they all agree that all of the different packaging formats and managers are a problem. However, is it really so? Most Linux distros are based on either RHEL, Debian, and Arch, which makes repackaging very easy, or even unnecessary. If you can find a package on one of the major distros, it is almost certain that it is on the others. Even independent Linux distros, such as Void Linux, Solus, Gentoo, and NixOS, don't seem to have any issues with packaging. As a developer, by simply using a free licence, you can just sit back and let all of the distros build binaries and do all of the work for you.

## There is no need for universal package managers

Many people point to the fact that universal package managers are necessary, because there is software that isn't mainstream enough to be on their niche Linux distro. Yet, there is a universal package manager that has been around longer than even traditional package managers. BUILDING FROM SOURCE! Many people forget that all of their software is a git clone, make, and make install away from being installed. While it may take longer to install, it is much faster and more efficient. And that's not even to mention the heaps of community repositories (AUR, xbps-src, OBS) that make installing software in the original binary form super easy.

## Universal package managers are inefficient

Flatpak, Snap, and AppImage are just not as fast as conventional package formats. Try using any modern version of Ubuntu, and just see how slow their Snaps are. But, that isn't really even the worst part. Because of the nature of universal package managers, they require much more space than traditional packages. Every single app, instead of sharing the dependencies of all other apps on the system, is bundled with all of its dependencies. This can add gigabytes of space to many apps, and slow down older HHD's.

# Conclusion

Universal package managers are often toted as the future of packaging on Linux. But in reallity, they are nothing more than a worse git repository you can use to build from source. And while they have a very small legitimate use in the server market, for apps on reproducable servers, the added stability is just not worth it when it comes to desktops. It doesn't make Linux less complicated and fractured, it just makes it worse.
