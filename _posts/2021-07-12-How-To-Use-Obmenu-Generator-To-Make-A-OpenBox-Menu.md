---
published: true
---
There are a lot of people that are switching to openbox. You can see why. It is fast, and endlessly customizable.  However, one of it's flaws is the menu. Openbox has a right click menu that isn't very good. While you could edit the config file yourself, there is a tool t assist you. Obmenu-generator is a piece of software that allows you to create a menu that actually has your applications. 

# Installation 

Obmenu-generator does not make it easy to install. However, you can install it on Arch, Debian, and all of their derivatives. Debain has a package on applications.opensuse.org. I will link that at the bottom. Or, if you use Arch/Manjaro it is available on the AUR. 

# Usage

It is fairly easy to use. You only need a few commands. It will allow you to make a static, or dynamic menu, with or without icons. Simply type these commands in your terminal depending on what you want. 

Static without icons:

	obmenu-generator -s

Static without icons:

	obmenu-generator -s -i

Dynamic without icons:

	obmenu-generator -p 
Dynamic with icons: 

	obmenu-generator -p - 


# Configuring 

You may notice that it has shortcuts for your file manager, web browser, and terminal. However, these don't always use what you want. There is a way to change these. You can do it right from the menu. In the menu follow this path, “advanced settings, obmenu-generator, menu schema”. This will open a text editor in the config file. For example, I don't like xterm. So I would search for “xterm” using the text editor, and replace it with xfce4-terminal. You can do this for anything you like. 

You should now have a working, static or dynamic menu for openbox, with your preferred applications. With obmenu-generator, the process has been made a lot easier, and less time consuming. So you can use OpenBox with a menu that is actually useful.

For Debian:  https://software.opensuse.org/download.html?project=home%3AHead_on_a_Stick%3Aobmenu-generator&package=obmenu-generator
