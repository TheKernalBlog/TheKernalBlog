---
published: true
---
When looking for a new Linux distro, there are a lot of options. Unless you are using something independent, you are going to have a distro with the package management system of RHEL, Debian, or Arch. However, there is some gray area where PCLinuxOS falls into. It is a super weird rolling release distro that I have has the pleasure of trying out. I am going to give my honest review of this distro, while pointing out its pros and it's shortcomings. 

## Installing 

PCLinuxOS has a very easy installer. It is a graphical Installer that almost anyone can use. The installer also has a lot of options when it comes to what software you would like. Even allowing you to download different iso’s and using them for the install. I personally love all of the options and the super easy install. 

## Package Management 

This is really the thing that makes this distro unique. It is rolling release like Solus, Arch, or Void. What most people are shocked to hear about though, is that it uses that apt package manager with .rpm packages. You may not expect it to work, but it uses the Debian package manager to download the same packages you might get with Fedora. PCLinuxOS has it’s own repos, and a surprisingly wide variety of packages. 

## Lack Of SystemD

You could probably figure out due to the fact that I use Void, that I am not the biggest fan of using Systemd. It is just a bit too bloated in my opinion. PCLinuxOS seams to share that sentiment as it uses Sysvinit. Sysvinit is what OpenRC is based off of. It is extremely minimal and extremely fast. While my boot time is around 15 seconds with Systemd, booting into PCLinuxOS only took about 5. Meaning that PCLinuxOS is great for anyone who wants a fast boot time. 

## Closed Source 

This is the thing that really stopped me from considering using this. I am a huge privacy fanatic, I even used to have a blog on privacy. PCLinuxOS ships with a lot of nonfree apps and drivers. Including Zoom, who illegally shared data with Facebook without consent. I would not recommend using PCLinuxOS if you switched to Linux mostly for privacy and security. 

# Conclusion 

While all of the foundations of a good operating system are there, PCLinuxOS is not something that I would recommend to most people. With the weird package manager that isn’t very polished, and the fact that it has little to no respect for your privacy, I would give this PCLinuxOS a pass. If you really want a Rolling release rpm distro check out OpenSUSE Tumbleweed, or Fedora Rawhide.

If you would like to check it out, here is the link to the official website. It is unclickable for your security. 

https://www.pclinuxos.com/
