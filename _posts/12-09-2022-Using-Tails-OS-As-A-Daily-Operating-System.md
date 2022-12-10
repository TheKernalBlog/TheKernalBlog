---
published: true 
---

<a id="org2b489f3"></a>

![img](/images/tails.png)

There are many reasons that someone would want to use Tails. Reporters use it to communicate safely, oppressed people use it to escape their state-controlled media, and of course, criminals use it to sell drugs. But, there's one use case for Tails that is rarely talked about, but surprisingly useful. Tails excels as a nomad operating system on a USB stick for people that either don't have a computer of their own, or have many computers that are a pain to sync. While yes, the ability to run on a USB with encrypted storage has the express purpose of increasing anonymity, after loosing my own computer, I have found Tails to be a huge convenience. And I'm going to explain how a fringe operating system for accessing TOR has completely changed  my everyday computing experience for the better.


<a id="orge0e929b"></a>

# How do I  use Tails?

For the past week or so, I've been using Tails for a lot of my regular activities, on a 64GB Micro Center USB drive. I've been using it on three machines, my broken laptop hooked up to a monitor, my fully-functional personal laptop, and my school-issued laptop. I've done a variety of schoolwork,  writing, and general internet browsing without a hitch on all three machines. All my files are stored locally on the USB drive, so as soon as I'm done on one computer, I can just boot out of it and start where I left off on another. 


<a id="org6f4420f"></a>

# What Software do I use?

Obviously, Tails has Tor, but a lot of people miss the general desktop applications that come with Tails. Things like GIMP, LibreOffice, Firefox (unsafe browser), and Audacity. In fact, I've been able to do almost every single day-to-day operation with exclusively the software pre-installed on Tails, plus a few quality of life applications. 


<a id="orgc87ed02"></a>

# How Do I  Install Software?

When I do want to install something, it's not as trivial as a simple `sudo apt install`, but it's still quite easy. There's two ways to do it; you can either install a deb application directly from the repo, or you can use Appimages. When installing a deb application, you're not actually installing it on the USB, you're simply telling Tails to re-install the package every single time that you reboot. Not only does this take a lot of time, but you need access to internet every single time you reboot for it to work. The much simpler solution is to use Appimage. You can place [Appimages](https://www.appimagehub.com/browse) in your persistent folder, and use them as regular applications. This is how I use VLC, yt-dlp, and even Emacs.


<a id="orgfdf27a1"></a>

# Why Should You Use Tails As Your Main OS?

Having your entire OS contained in a USB stick is very convenient. If you have access to any public computer, you can use it while still having access to all of your files, programs, and app data. They're not library computers or school computers anymore, they're <span class="underline">your</span> computers. And if you're going to someone else's house, you can just bring your USB stick instead of trying to cram a whole laptop into your bag. It's very practical. 


<a id="org0138564"></a>

# Why Shouldn't You Use Tails As Your Main OS?

Simply put, while you can do most of your work in Tails, it's not nearly as efficient as a locally installed operating system. There's almost no chance for customization, you're limited in what apps you can install, and on top of that, you've got significantly less storage. For that small bump in convenience, you are loosing a lot of features. Plus, by carrying your entire operating system in a USB drive, you're increasing the chances that you loose or break it by a lot, which could wipe out your entire operating system with something as trivial as an unzipped zipper on your bag. 


<a id="org2e0951a"></a>

# Conclusion

Tails as a daily operating system is not conventional, but it's an excellent use case. I don't think I'm  going to continue to use it as my main OS, but I do think that a live Tails USB will be essential in my travel bag from now on. It's an amazing operating system for daily use. Whether you're a nomad, a student, or work in multiple offices, Tails can be the perfect solution to all of your file-syncing problems. 

# Table of Contents

1.  [Introduction](#org2b489f3)
2.  [How do I  use Tails?](#orge0e929b)
3.  [What Software do I use?](#org6f4420f)
4.  [How Do I  Install Software?](#orgc87ed02)
5.  [Why Should You Use Tails As Your Main OS?](#orgfdf27a1)
6.  [Why Shouldn't You Use Tails As Your Main OS?](#org0138564)
7.  [Conclusion](#org2e0951a)
