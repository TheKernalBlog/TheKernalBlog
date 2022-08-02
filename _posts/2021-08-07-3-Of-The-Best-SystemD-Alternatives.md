---
published: true
---

When using an init system with Linux, you are most likely going to be using Systemd. Systemd is what comes with the majority of Linux distros as of current. However, there has been a lot of criticism against Systemd. Luckily, there are other init systems that you can use. I am going to provide some of the alternatives, and you can decide for yourself what you would like to use as a init system. 

# OpenRC 

OpenRC is the init system of choice for Gentoo, and it is loved by many. It is known for being super fast and simple. All of the configuration is done by shell scripts, meaning that you can add and remove services easily. It was built off of another init system called sysvinit, adding more features while still staying super minimal. 

# runit

runit is the init system of choice for Void Linux, the Linux distro that I am currently using. It is very minimal, version 1 is contains just 274 lines of code. One of the best things about it is that it basically launches all of the system services at the same time, meaning that the boot speed is ridiculously fast. Like OpenRC, adding new services is also really easy. It really sticks to the unix philosophy of oing one thing and doing it well. 

# s6

The only Linux distro that I could find currently using s6 is Artix Linux. A lot like Systend, s6 is not one script, it is made up of 6 services. The thing that makes it so good is the fact that you can bundle applications for startup together Meaning that you will have a very fast boot time. Sometimes it is faster than runit. 

# Conclusion 

While these are not the only alternatives to Systemd that there are, they are the ones that are most used. I would recommend that if you want a faster boot time and less bloat, that you ditch Systemd for a Systemd free Linux distro, or simple changing the init system on your current Linux distro. 

If you would like to more research yourself, here are the some websites where you can learn about these init systems. (Unclickable for your security) 

OpenRC: https://wiki.gentoo.org/wiki/Project:OpenRC

rinit: http://smarden.org/runit/

s6: https://wiki.artixlinux.org/Main/S6
