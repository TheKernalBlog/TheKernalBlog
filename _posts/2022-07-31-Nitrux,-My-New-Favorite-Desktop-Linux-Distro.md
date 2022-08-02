---
published: true
---
There are hundreds of desktop Linux distros that attempt to improve on many aspects of the experience. However, it is very rare that a distro truly distinguishes itself from the rest. Nitrux does just that. With an unusual base, underused init system, and even custom app framework, Nitrux still manages to be extremely fast, reliable, and idiot proof. So, I'm going to give you a little bit deeper of an explanation about what makes this distro so great.


<a id="orga0bd740"></a>

# Install

![IMG1](/images/NitruxInstall.png)

The install process for Nitrux seems to be especially polished when compared to other distributions. They use a customized Calamares installer that's super clean and professional. It has all of the features that you could ever wish for in an installer, all packed into a super slick, modern interface. It makes the new Windows installer look like it has come strait out of 1995. 


<a id="org81994fa"></a>

# Desktop

![IMG2](/images/NitruxDesktop.png)

As you can see, the default Nitrux desktop is absolutely stunning. But if you look closely, you'll see that the desktop is just a heavily themed KDE, making use of Latte instead of traditional KDE panels. Functionally, it's almost identical to MacOS, which you may or may not appreciate. And while it looks amazing, I would not say that it's the most stable, especially on lower end hardware, as the panel crashed on me twice in just 30 minutes in my VM.


<a id="org5261016"></a>

# Resource Usage

![IMG3](/images/NitruxResources.png)

Nitrux is surprisingly light on resources. On a cold boot, with no programs open but the terminal, I was registering 750-800MB of RAM usage, and less than 2% total CPU usage on my 4GB 4 core virtual machine. While that may be a little less than what some older computers can reasonably handle, for the extremely polished, heavily themed KDE desktop you get, that's pretty darn great. 


<a id="orga2779ca"></a>

# Nitruxs's Base

Nitrux, instead of choosing Ubuntu as it's base, opts for Debian Sid, which is an amazing decision. However, it's not just your bogstandard Debian Sid. Nitrux swaps out the industry standard init system, Systemd for the more optimized, less common OpenRC. They also seem to use some external repositories for KDE Neon. It may not be one of the main selling points of the distro, but it is their choice of distro base that really sets Nitrux apart from the hundred other Ubuntu forks. 


<a id="orgf621305"></a>

# MauiKit

![IMG4](/images/NitruxFile.png)

MauiKit is the thing that really puts Nitrux on the map. Maui is a cross platform app toolkit that is beautifully integrated into the OS. Many of the apps that would otherwise be native apps from KDE, are replaced with Maui alternatives. Everything from the file manager, the terminal emulator, and even the music player are completely re-written in MauiKit. And although I didn't use many of the apps for more than a minute, I found them all extremely snappy and beautiful.

Even if you don't intend to use Nitrux, I would recommend that you check out some Maui apps right [here](https://mauikit.org/apps).


<a id="org6bc0359"></a>

# Package Management

![IMG5](/images/NitruxAppStore.png) 

Nitrux handles  package management exceptionally well. They discourage the use of traditional binary package managers, but refreshingly, they tend to lean twords Appimages as their main method of distributing software. All of the Maui kit apps and most of the pre-installed software is packaged in Appimage. And unlike some other Appimages I've used in the past, Nitrux's seem to launch almost instantly. However, if you want to install Deb packages, you are required to use their 'pkcon' at the terminal as an alternative to the standard apt package manager. 


<a id="org2f7565e"></a>

# Conclusion

Nitrux is one of a kind. It's an incredibly powerful distro that has cemented its place not only as a viable alternative to Windows and MacOS, but as an easy to use alternative to most desktop Linux distros. You can tell that Nitrux has had a lot of hard work put into it, which is the reason that it feels so polished and well thought out. If you're looking for a simple, easy to use desktop distribution, but are less than impressed by most of the options, I would 100% recommend giving Nitrux a shot. 


# Table of Contents

1.  [Install](#orga0bd740)
2.  [Desktop](#org81994fa)
3.  [Resource Usage](#org5261016)
4.  [Nitruxs's Base](#orga2779ca)
5.  [MauiKit](#orgf621305)
6.  [Package Management](#org6bc0359)
7.  [Conclusion](#org2f7565e)
