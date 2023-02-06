---
published: true
---

ARM is taking over the world. There are an estimated 6.8 billion people in the world walking around every day with an incredibly ARM powered computer in their pocket. And while the smartphone market is entirely focussed on these cheaper, more efficient chips, desktop & laptop computers are almost all still using Intel x86 processors. But, there are exceptions. Especially in China, there are hundreds of ARM laptops & desktops being produced every day that bring powerful, affordable computers to the masses. And the primary operating system being used on these computers? Linux. So, as someone who owns one of these ARM laptops, I believe I'm in a position to fairly judge some of the Linux distros that I've personally tried, and give some recommendations as to what Linux distro could fit your needs best.

# Manjaro 

Manjaro is the OS that shipped with my Pinebook Pro, and if you've read my other blog on the subject, you'd know that I did not have the best experience. But still, even though my initial impression may not have been the best, it's hard to dislike Manjaro. The truth is, in most cases, you just can't beat it. Manjaro ships with 5 different desktop environments, a ton of very sensible applications, and amazing hardware support. Like all ARM distros, the install was a little more complicated then I'd have hoped, but apart from that, everything was super simple. With other ARM distros, I've had to spend hours fiddling around with kernels and drivers before I could get it into a usable state. But, when I install Manjaro, I know I don't have to worry about it. 
However, that convenience comes with a cost. Manjaro is, at least from my experience, incredibly unstable. Now, being based on Arch, you wouldn't expect it to be perfect, but I've installed Manjaro on both x86 & ARM systems, and I've faced a ton of issues. I've had unfixable package conflicts, WiFi bugs, and I've even had the bootloader completely fail on me a couple times. So if you're considering Manjaro, be sure to take that into account.  

# Armbian 

You may not be surprised to learn that currently, I am writing this very blog on Armbian. And out of all the ARM based distros that I've tried it is by far the most stable. It's a lot like Linux Mint in the regard that it ships both an Ubuntu version and a Debian version with various different desktop environments. But it's also a little like Slackware in the sense that it ships with well over 50 graphical applications for doing anything you could ever desire.  

Some of the most appreciated additions are the Armbian instillation, configuration, and debugging tools. The installer and configuration tools are both built with ncurses, and extremely useful. You can change kernels, install firmware, and update your system without having put in any real effort. It's one of the best configuration tools that I've used in a very long time. 

But, there are some things that are lacking. On the Pinebook, even with the newest kernel, I can't seem to get Bluetooth to work, and USB-C DP output is extremely buggy. It makes sense, because Armbian has comparatively a lot less contributors that Manjaro, and a wide range of devices to support, but for such a popular laptop I hoped that some of these problems would be ironed out by now.  

# Q4Os 

Q4OS is an extremely interesting Debian based distro that I've had my eyes on for a while. It's well known in the Linux community for reviving old 32 bit machines with its desktop environment Tritiny. But it seems like they are trying to expand into the ARM market. And before I tried Armbian, I tried Q4OS on a SD card and had a pretty nice experience. 

However, there is one glaring issue with the Q4OS ARM port. There actually isn't one. Q4OS works on ARM, and it has all the same features as the X86 version, but there is no actual image for you to install. In order to get Q4OS running on an ARM device, you must first install Armbian/Debian, then run a script that will switch your repositories and install the Q4OS desktop on top of your pre-existing system. Not only is this a hassle, unless you're super keen on Trinity, you can just install the KDE version of Armbian for an extremely similar experience. 

But, if you ignore all that and just look at the face value of Q4OS, it's not bad. It's rock solid, fast, and very easy to use. When you use it, you get the impression that it was made for a much much simpler, more efficient time. Where everything does its job and you don't have to dumb things down with smooth, flat designs and big buttons. And if you want to emulate Windows ARM applications, Q4OS comes with a very easy to use Wine GUI. And even with KDE, it runs at 450mb and 5% CPU usage on a cold boot on my Pinebook Pro. It's great, but just not for me. 

# Conclusion 

I still believe that ARM distros are merely in their infancy. ARM laptops may not be new, but they are yet to explode in popularity. And as the demand for laptops grow, and the price of ARM chips go down, it's inevitable that ARM chips take over. And much like Linux's growth originally coincided with the popularity of the Intel x86 chipset, new, better ARM distros are going to rise out of the ashes. And while no ARM distro is truly the best, they're are certainly some that stand out from the rest, and I feel that all three of these distros are great options that you should really consider when buying and investing in an ARM machine of any kind.  
