---
published: true
---
It is no doubt that Fedora is steadily becoming an amazing option for desktop Linux, in many cases outperforming Ubuntu and OpenSUSE. And yet, despite its amazing features, great support, and beautiful default experience, there always seems to be some things that aren't there. Many desktops, multimidea codecs, and non-free applications are not available on Fedora Linux by default without some heavy tinkering. And it is that problem, that Ultramarine Linux attempts to solve. Ultramarine Linux is a Fedora based, open sourced distro that attempts to make the experience more usable by adding the option for more desktops, external repositories, and codecs that aren't available on the regular Fedora. So, after giving it a spin, I'm going to show you what makes Ultramerine tick, and why you might want to check it out. 

# Desktop Environments

In an attempt to differentiate itself from Fedora, Ultramarine features basically all of the desktop environments that Fedora doesn't. Currently, it features these 4 desktops.  

- Budgie (Flagship) 
- Pantheon 
- Cutefish 
- GNOME 

From my testing, in which I just used the flagship Budgie edition, they do very little to change how the desktop works, other than applying their own icon and GTK themes, called "Fluent Round".  

# Resource usage 

Unsurprisingly, the resource usage of Ultramarine is almost identical to that of Fedora, hovering around 1-2% CPU usage and 250-300mb of RAM on my 4 core 4GB of ram virtual machine when Xorg isn't running. However, with the flagship Budgie, I found Ultramarine staying around 900-950mb of RAM and 4-5% CPU usage, which isn't too bad considering how heavy Budgie can be. 

# Applications 

Ultramarine contains everything but the kitchen sink. It has a graphical tool for everything, from a wallpaper randomizer, system log viewer, password manager, and more. But, thankfully, unlike may Linux distros, none of these applications are useless, unwanted, or random. They all serve a specific purpose that helps you manage your system. Plus, instead of Bash, Ultramarine opts for ZSH with a custom theme, which, in my opinion, is a pretty great choice. 

# Converting Fedora to Ultramarine 

One nifty thing that Ultramarine does, is provide a simple shell script that will convert a regular Fedora installation into a Ultramarine installation. This will enable all of the 3rd party repositories, and give you the option to install and use Cutefish, Pantheon, and Budgie. If you would like to convert, you can just use this command, ensuring that you have 'curl' installed. 

	bash <(curl -s https://ultramarine-linux.org/migrate.sh)

# Conclusion 

Ultramarine, is, with no doubt, a great operating system. It has enough tools to make developers happy, it's easy enough for a total Linux beginner, and features a vast amount of features and packages that you won't find in Fedora. If you are one of those people who wants a usable, powerful, easy to configure system with a little bit of nonfree software, Ultramarine may be just what you've been missing in Fedora.
