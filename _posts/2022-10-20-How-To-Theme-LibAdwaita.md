--- 
published: true
---

GNOME's switch to Libadwaita has been a little controversial. Many people have complained about how GNOME is taking away people's option to theme their desktop. And while, the goal was to empower developers by restricting the customizability of GTK3, it's not all gone. There is in fact, ways to customize GNOME 42. And if you're interested in doing some ricing, I'll show you how you can download, install, and apply GTK4 themes to Libadwaita applications.  

# Manual Themes 

## Downloading the LibAdwaita theme 

Surprisingly, there are quite a few themes that now support theming LibAwdaita. But, I personally found a pretty good [github repo](https://github.com/odziom91/libadwaita-themes) that has plenty of themes that seem to work. If you have git, just copy this command into the terminal. 

	git clone https://github.com/odziom91/libadwaita-themes

## Applying the LibAdwaita theme 

You can use your file manager to unzip and move the theme file in a GUI, however, I'd recommend just typing these four commands into the terminal. 

	cd libadwaita-themes/THEME

	unzip THEME.zip

	rm -Rf ~/.config/gtk-4.0

	mv gtk-4.0 ~/.config

And tada! It works! 

![IMG1](/images/ManualThemeWorks.png) 

# Automatic Theming 

If you're not looking to use a specific colorscheme, but still want a little bit of customization in your desktop, this is the way to go. Using Gradience, you simply upload your wallpaper, and get an automatically generated theme that applies to LibAdwaita and gtk-adw3. Gradience maintains the LibAdwaita look while changing the colorscheme, ensuring stability. To start, just install with Flatpak. 

## Installing Gradience 

	 flatpak install com.github.GradienceTeam.Gradience

## Downloading adw-gtk3

Then, I'd recommend installing the gtk-adw3 theme. This is a theme that replicates the look of LibAdwaita in GTK3 applications. But most importantly, gtk-adw3 is able to be themed by Gradience. Just go to the official [github repo](https://github.com/lassekongo83/adw-gtk3/releases/tag/v4.0) and download the most recent tar file. Then, move it to the *.themes* directory and apply it. 

	tar xf adw-gtk3v4-0.tar.xz
	
	cd adw-gtk3v4-0
	
	mv adw-gtk3 ~/.themes
	
Apply it, 

![IMG2](/images/Tweaks.png) 

and then launch gradience.

## Using Gradience to set the colorscheme 

 Gradience is dead simple to use. All you need to do is go over to the ***Monet*** tab, and upload your wallpaper where it says, 'Background Image'. From there, you can choose between a light and dark theme and manually change some of the colors that you don't like. Once you've got your colorscheme, hit 'apply', check the box next to 'GTK3 Applications', and set the theme. 
 
 ![IMG3](/images/GradienceWorks.png) 

# You're Done 
 
 Now, you've got a fully customized GNOME desktop that adheres to any theme you could ever imagine. While the decision to restrict theming with Libadwaita may be controversial, at least now there's a way for people who dislike the change to rice their desktops. Worst case scenario, you break everything and go back to the already beautiful default theme. 
