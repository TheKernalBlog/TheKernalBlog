---
published: true
---

<a id="orge0800db"></a>

![img](/images/EXWM.png)

About a week ago, I was sitting in my Science class after finishing a review. Having nothing better to do, I whipped my laptop out of my bag and started fixing any grammar/spelling mistakes in the blog I had finished the day before. Eventually, my teacher came around and saw me reading over my blog. He was a bit confused, but, having worked with Ubuntu in the past, we got talking about Linux, and for almost 10 minutes, he sat there asking questions as I explained my setup to him. So, I figured, if my 70 year old science teacher was able to stand my long-winded, fairly boring breakdown of every individual part of how I set up my Linux distro, the internet might want to know too. And so, I am going to break down every important component of my setup, what everything does, and how I use it. Hopefully, seeing how I setup my computer can give you some ideas and inspire you to try out some of the same stuff as me.


<a id="orgf80ca78"></a>

# Hardware

Right now, my main computer is a small, Acer Aspire with 2GB of RAM and 2 CPU cores. It's not the best hardware in the world, but with most of the software that I run, it's a non-issue. My only gripe with my laptop right now is that Linux is not automatically added to the boot menu when installed, but you can still manually choose the efi file to boot from.

Apart from the laptop itself, my desk setup is pretty great. I have a 1920x1080 Acer monitor, a Logitech G413 mechanical keyboard, a vertical mouse from a random Chinese company, and a super slick pair of Altec Lansing speakers with a giant subwoofer that my school was going to throw away.


<a id="orgd13cbff"></a>

# Operating System

Although I have been known to distro hop on occasion, I've been using Fedora the longest. It's rock solid, pretty up-to-date, and easy to configure. I've been using it for a year and a half , and it hasn't crashed on me once. 


<a id="org8e65aa3"></a>

# Window Manager/Desktop Environment

EMACS!!!! Thanks to [EXWM](https://github.com/ch11ng/exwm), I am able to log directly into Emacs. I wouldn't recommend that everyone use EXWM, as it requires fairly comprehensive Emacs knowledge, but as someone that uses Emacs for most things anyway, it's extremely convenient.

In the past, I've used Polybar for a system tray and propper workspace monitor, but recently I've found myself pretty happy with just a [customized modeline](https://github.com/milkypostman/powerline). However, if you do want Polybar integration in EXWM, I'd check out System Crafter's amazing [guide](https://www.yewtu.be/watch?v=usCfMstCZ7E&feature=youtu.be) on how to set it up.


<a id="org8fb7be2"></a>

# Password Manager

After over a decade of using the exact same password for all of my accounts, this was the year that I finally got a password manager. And after a little bit of deliberation, I chose KeePassXC. You get all of the conveniences of a cloud based password manager, while all of your passwords remain safe locally on your device. If you want more information, check out the [blog](https://thekernal.xyz/2022/12/01/Abandon-Your-Browsers-Password-Manager-And-Switch-To-KeePasXC/) I wrote the other day.


<a id="org95e2da0"></a>

# Multimedia System

I've used every single open source multimedia system that Linux has to offer. But, like most people, I use VLC. It's fully open sourced, and yet can reliably play more files than any other media player with absolutely no struggle. Hell, even most Windows users recognize how amazing VLC is. 


<a id="orgeeb1548"></a>

# Browser

There are a plethora of amazing web browsers out there (Ungoogled-Chromium Epiphany Falkon) but, after giving all of them a fair try, I have chosen to stick with regular ol' Firefox. For privacy, I use the [Arkenfox](https://github.com/arkenfox/user.js/) user.js with Noscript, Ublock Origin, Cookie-autodelete, and SearX. And out of hatred for *modern* UI, I use this [CSS theme](https://github.com/leadweedy/Firefox-Proton-Square) to bring back the Firefox Quantem look. By the time I'm done with it, Firefox doesn't really look the same, but that's what I like about it so much. There's nothing stopping me from completely destroying the default functional, slick browser and turning it into a twisted imitation of its former self.


<a id="orgc71fb84"></a>

# Shell

For the most part, I use standard bash. I've played around with Fish & Zsh, but I really don't see much reason to use them. It's already very functional, but I do like a little bit of eye candy, so I used [oh-my-bash](https://github.com/ohmybash/oh-my-bash) to get my beautiful Half life theme. And although I use bash most of the time, I also occasionally use Eshell within Emacs. It's Elisp integration is incredibly useful in a wide variety of cases, but the fact that you can't run Eshell in a propper terminal buffer means that it's a no-go for me most of the time. 


<a id="org43736ac"></a>

# File manager

I use two file managers. Dired & Thunar. Obviously, when working within Emacs, Dired is king. It's surprisingly powerful, and integrates amazingly with all of the Emacs modes for PDF's and image files. But, Thunar is my go-to when it comes to mounting USB drives and my phone. Sure, I could use the terminal to manually mount my phone onto my file system every time I want to add another mp3, or I can just open Thunar and have it automatically mount without any fuss. Thunar is seriously a huge convenience. 


<a id="org9ffa747"></a>

# Text Editor

Emacs! I know, it's a bit silly to list Emacs separately when I use it for so many unrelated things, but I feel like Emacs needs to be recognized for the powerhouse of pure text editing it is. I swear, there's absolutely no compromises when it comes to text editing in Emacs. I can write everything in one markup language, and export it to any file format I desire, all while having access to every single quality of life feature that might be missing from any other similar editors. I've never used anything else quite like it. 


<a id="org366bd2b"></a>

# Conclusion

Now, you should have a good idea on what I use on a daily basis. Sure, half of it's just Emacs, and the other half is quite basic, but I think that every singe piece of software mentioned is worthwhile and definitely worth considering. If there's something in here that stands out to you, I'd urge you to give it a try. I swear it'll make your computing experience at least a little bit better. And plus, you've read the entirety of this blog post, and you don't even have the excuse of being my Science teacher, so I know that you have enough free time on your hands to implement many of these programs into your life. 

# Table of Contents

1.  [Introduction](#orge0800db)
2.  [Hardware](#orgf80ca78)
3.  [Operating System](#orgd13cbff)
4.  [Window Manager/Desktop Environment](#org8e65aa3)
5.  [Password Manager](#org8fb7be2)
6.  [Multimedia System](#org95e2da0)
7.  [Browser](#orgeeb1548)
8.  [Shell](#orgc71fb84)
9.  [File manager](#org43736ac)
10. [Text Editor](#org9ffa747)
11. [Conclusion](#org366bd2b)
