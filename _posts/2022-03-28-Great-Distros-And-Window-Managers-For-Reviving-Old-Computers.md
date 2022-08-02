---
published: true
---
It happens to all of us, we are cleaning out our attic, garage, or other abandoned place in our house, and you find a super old computer. Whether it is a single core 300 MB Dell laptop, or a ancient IBM desktop, it is a shame to see all of these computers go to waste. In many cases, the only way to get these computers back into working order is by installing a Linux distro with the correct software. So, to get the most out of your old computers, I am going to explain some of the best options for reviving most aging and abandoned computers.

## Distros

Obviously, when discussing how to revive old computers using Linux, one of the most important things to consider is the distro that you decide to run. If you have a decent amount of memory, you should be just fine using the i386 version of popular Linux distros like Arch, Debian, or even Fedora. Yet, if you have a very limited amount of RAM, such as 500mb, I would recomend looking at some of the lighter options. Here are the distros that, in my experience, are some of the lowest when it comes to memory & CPU usage.

### Void Linux

This is my personal recommendation. Void Linux is probably the least bloated Linux distro that has been released in a while. In my experience, without Xorg or any additional processes running, it lingers around 150mb on my 8GB main system. Plus, if you are planning to run it without a graphical environment, it has a TUI installer and a surprising amount of packages you would find on any server distro.

### Antix

Antix has been recommended by the Linux community as a great Linux distro for old computers for a very long time. It is a Linux distro that it based off of Debian, that doesn't use Systemd. It also comes with four pre-configured window managers. With no Xorg or other additional packages running, I report memory usage at around 140mb on the same machine, which is very impressive.

## FreeBSD

While I mainly try to stay away from BSD, as this is a Linux blog, I can't help but recommend FreeBSD for this job. FreeBSD is known for reviving old computers, and in my testing, runs on my computer while using around 200mb of RAM. Plus, you can do all of your configuration with a graphical TUI application, which does not require Xorg.

## Window Managers

Unless you are planning to use your old computer as a server, you are going to want a window manager. There are many out there that would fit the requirement of being lightweight, but I am going to list 3 window managers that are extremely light.

### DWM

I may be a little biased, because I am using DWM right now, but it really is extremely lightweight. The whole point of DWM is to have a very small footprint with the least amount of code. So, it is no surprise that it is extremely lightweight. It only ever uses less than 1% of my CPU, and only around 10mb of RAM.

### IceWm

If you would like a standard desktop experience as opposed to a tiling window manager, IceWm is the best option. It has a regular Windows95-like desktop experience. It has a system tray, start menu, and window list. But just because it is fully featured, doesn't mean that that isn't super lightweight. It only takes about 20mb of RAM, which is very impressive due to the amount of functionality that it has.

### i3

If you are a beginner, who doesn't know a lot about tiling window managers, i3 is great for you. While you still have to edit some config files, you don't have to know any coding, and the syntax is very easy to understand. Plus, the resource usage is nothing to scoff at either. On my system, i3 was only using around 15mb.

# Conclusion

While many people would just discard many perfectly good computers, not even realizing that they still have their uses. By rescuing these unused machines, you can not only get a free computer to do with as you wish, but you can also cut down on the amount of electronic waste. So, you can get that 'crappy' old laptop from your attic, and use it as a web server, testing machine, or even general purpose computer.
