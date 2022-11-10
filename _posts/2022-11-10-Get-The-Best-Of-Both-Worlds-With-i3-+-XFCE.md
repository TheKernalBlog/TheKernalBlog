---
published: true
--- 

![Image0](/images/i3XFCE.png)

Recently, after the death of my Dell Latitude 3400, I've had to completely re-build my setup on an older netbook from 2014. Now, as you can imagine, it's not the best computer in the world. It only has 2GB of RAM and 2 CPU cores. I started using XFCE, and I was quite happy with how well it worked and how easy it was on the resources. But I still yearned for tiling. Now, on GNOME, this would be as easy as installing pop-shell and calling it a day, but that's a little more complicated with XFCE. So, after trying a few tiling scripts, I thought, "Why not use the real thing"?. And guess what, it works. You can install i3, and replace XFWM seamlessly. Now, it requires a little trickery, but if you're intrigued, I'll show you how you can remove XFWM and use a tiling window manager with all of the perks of XFCE. 


# Installing i3 and Nitrogen 

Obviously, you're going to need to install i3, but if you want to have a desktop wallpaper, you're also going to have to install Nitrogen. So, just in case you don't know the command, or are just too lazy to type it all out, you can copy-paste one of these commands into your terminal. 

## Ubuntu/Debian 

    sudo apt install i3 nitrogen 

## Fedora/CentOS

    sudo dnf install i3 nitrogen 

## Arch Linux 

    sudo pacman -S i3 nitrogen 

## OpenSUSE 

    sudo zypper in i3 nitrogen 

# Removing all of the keyboard shortcuts 

XFCE has a variety of useful keyboard shortcuts pre-set. And while this is pretty useful when using XFWM, the keybindings can conflict with keybindings from i3. So, it's best to remove them all. All you need to do is open the settings manager, and select Keyboard --> Application shortcuts. From there, you just manually remove them all. 

![Image1](/images/Shortcuts.png) 

# Removing XFDesktop and XFWM 

XFWM and XFdesktop serve two very important roles in XFCE. XFWM is the window manager itself, and XFdesktop handles the wallpaper & right click menu. Sadly, both conflict with i3, so they need to go. And it's surprisingly simple to get rid of them. Again in the settings manager, under Session and Startup --> Current session you'll see both running. To the right, you'll see a little section under 'Restart Style'. While it may not look like it, you can actually click on the text boxes. Click on the restart styles for XFDesktop and XFWM respectively, and switch them both to 'Never'. Then, hit 'Save Session'. 

![Image2](/images/ByeByeXFWM.png) 

# Starting i3 

Don't close out of your session settings yet. You still need to start i3. It's as simple as going to 'Application Autostart' and clicking on the plus button to make a new entry. Name it 'i3', put 'i3' as the command, and start it on login. It should look something like this. 

![Image3](/images/Helloi3.png) 

# Configuring i3 

Technically, you're ready to log out and log back in to XFCE with i3. But in reality, you've still got a long ways to go before you're out of the woods. You still need to make a config file, and change a few settings. In order to get the i3 config file, you've got two choices. You can log into a i3 session and let the i3-wizard create the config file for you, or you can copy the default config from the internet. If you're going to go the second route, you need to create the directory 

## Obtaining a config file 

    mkdir ~/.config/i3 && cd ~/.config/i3 

and then create the config file, 

    touch config 

before opening it up in your text editor of choice. 

    EDITOR config 

Now, just copy-paste the contents of [this](https://github.com/sainathadapa/i3-wm-config/blob/master/i3-default-config-backup) file, and you're ready to edit. 

## Removing the panel 

Since you're going to be running xfce4-panel, there's no use for i3 to have a panel. So, comment out these lines like so. 

```
#  bar {
#          status_command i3status
# } 
``` 
## Replacing Dmenu 

Dmenu is nice, but it pretty obviously doesn't fit in with XFCE. Thankfully though, not only is it easy to change, the best alternatives are build directly into XFCE itself. Find this line, 

    bindsym $mod+d exec dmenu_run

and replace '**dmenu_run**' with the XFCE appfinder. 

    bindsym $mod+d exec xfce4-appfinder 

Or, if you'd prefer, you can use Whiskermenu instead. 

    bindsym $mod+d exec xfce4-popup-whiskermenu 


# Using a wallpaper 

With XFDesktop gone, you'll find yourself booting into XFCE to be met with nothing but a panel and a black screen. While this is technically functional, most people would prefer to have a desktop wallpaper. Thankfully, with Nitrogen (which you should have installed earlier) it's a piece of cake. Just launch Nitrogen, add a folder, and select your wallpaper to apply it. Then, going back to Session and Startup --> Application Autostart, and create a new entry that runs 'nitrogen --restore'. It should look like this. 

![Image4](/images/Wallpaper.png)

# You did it!

If you followed the instructions, you should now have a completely functional tiling desktop environment using XFCE and i3. Is it the most minimal? No. Is it the most functional? No. But, if you like tiling window managers, it's the closest you can get to a complete DE with decent tiling functionality. This way, you don't have to spend hours getting Wifi, Bluetooth, Notifications, or anything else to work with regular i3. 
