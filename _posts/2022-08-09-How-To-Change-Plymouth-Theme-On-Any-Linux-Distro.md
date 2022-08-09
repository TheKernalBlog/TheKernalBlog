---
published: false
---
Chances are, if you use desktop Linux, you're using Plymouth every time that you boot into your computer. Whether you use Fedora, Manjaro, Debian, or Ubuntu, Plymouth is going to come pre-installed. Plymouth, is a boot screen application that gives you something a little more appealing than a simple Systemd output. However, on most distros, it's a little stale. Thankfully though, there are a plethora of themes available, and I am going to show you how you can install and apply them to any Linux distro.


<a id="org6a3d2f6"></a>

# Installing Plymouth Themes

![IMG1](/images/PlymouthTheme2.png) 

There are a ton of Plymouth themes out there for you to choose from. Depending on what Linux distro you use, there are going to be a ton in the repositories. But, there are also hundreds of themes made by contributor and theme designers available to download online. My personal favorite place to grab Plymouth themes is [Pling](https://www.gnome-look.org/browse?cat=108&ord=latest), but there are many more on Github, Deviantart, and scattered around random parts of the web.

If you want to install some simple, generic themes from your distro repositories, feel free to copy-paste one of the commands here, while making some considerations depending on what distro you use, and what themes you would actually like installed. 


<a id="org91c8bb0"></a>

## Using Distro Packages


<a id="org7a0f8d4"></a>

### Ubuntu/Debian

`sudo apt install plymouth-themes`


<a id="orgd51c527"></a>

### Fedora

`sudo dnf install plymouth-theme-charge plymouth-theme-hot-dog plymouth-theme-solar plymouth-theme-spinfinity plymouth-theme-fade-in plymouth-theme-script plymouth-theme-spinner`


<a id="org28058b9"></a>

### Arch Linux

`Comes with themes pre-installed Plymouth package` 


<a id="org6bf390d"></a>

## Using A Theme From The Internet

Once you have your theme downloaded and extracted, all you need to do is put it in the right place. You can either use a graphical file manager with root privlages, or a terminal. Just move the directory to **usr/share/plymouth/themes** in the file manager, or use this command to do the same thing from the terminal.

`sudo mv PATH/TO/THEME /usr/share/plymouth/themes/`


<a id="orgd907530"></a>

# Switching Default Theme

![IMG2](/images/PlymouthTheme3.png) 

Once you have the directory containing the theme in the correct place, all you need to do is enable it. And while there are many guides that will show you distro specific ways of changing the default theme, I personally think this method is better, because not only is it dead simple, it works on every Linux distro.

First, in your terminal emulator, you need to cd into the directory where you installed the theme. 

`cd /usr/share/plymouth/themes/THEME`

Then, in that directory, you can type `ls`, and you will see a file that ends in *.plymouth*. Once you've identified the file, all you need to do is copy it to the *default.plymouth* file, using this command.

`sudo cp THEME.plymouth /usr/share/plymouth/themes/default.plymouth`


<a id="orgd612952"></a>

# You're Done!!

All you need to do now is reboot, sit back, and admire your new plymouth boot screen. The possibilities are endless. You can use a theme that blends with your display manager, one that fits the theme of your desktop, or one that shows some more information than just a spinning circle. Whatever the theme you choose, the boot screen is your oyster, and you can do with it what you wish. 


# Table of Contents

1.  [Installing Plymouth Themes](#org6a3d2f6)
    1.  [Using Distro Packages](#org91c8bb0)
        1.  [Ubuntu/Debian](#org7a0f8d4)
        2.  [Fedora](#orgd51c527)
        3.  [Arch Linux](#org28058b9)
    2.  [Using A Theme From The Internet](#org6bf390d)
2.  [Switching Default Theme](#orgd907530)
3.  [You're Done!!](#orgd612952)
