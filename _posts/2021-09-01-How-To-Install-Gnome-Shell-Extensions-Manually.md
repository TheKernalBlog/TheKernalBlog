---
published: true
---
Gnome is a very controversial desktop environment. However, it is the one that I currently use. One of the main things that brings people to the desktop environment is the “shell extensions”. These are little bits of code that allow you to tweak your desktop. If you are going to install them the normal way, you will need to install their web browser extension. However, there is a way that you can install them manually without ever having to touch a browser extension. I am going to show you how to install them yourself by downloading the zip file and adding it yourself. 

# Download The Extension 

To use the extension, you are obviously going to want to get them from the <a href="https://extensions.gnome.org/">Offical Website</a>. You will be prompted to install the browser extension, but there is no need. Then find the shell extension that you want to install, and then downlaod the latest version. As an example, I am going to install the “Just Perfection” extension. 

# Extract The Zip File 

You are going to have to extract the zip file of the extension that you just downloaded. The easiest thing to do would be to go to your file manager, and use your archive manager to extract it. However, if you would like to extract it using the terminal you can use these two commands. 

	cd Downloads

	unzip NAMEOFFILE.zip 

# Rename The File 

If you were to just move the file to the correct directly currently, it would not work. You are going to need to rename the file that you just extracted. To do this, you need to find the “UUID”. Don’t worry, its not hard. Simply go into the file you just extracted, and open the “metadata.json”. You will see a line that has “UUID:” followed by the UUID itself. In my case, “just-perfection-desktop@just-perfection”. Then, you will have to rename the file that you extracted the exact same as the UUID. 

# Moving the file 

Now is the fun part. You are going to move the extension to the extension file. If you are using the file manager, press “Ctrl+h” to show hidden files. Take your file, and cut/copy it to /home/.local/share/gnome-shell/extensions. If you would like to move it with the terminal, you can use this command. 

	mv NAMEOF@FILE ~/.local/share/gnome-shell/extensions 

Then restart the Gnome shell by logging out, and then logging back in. 

# Conclusion

You should now be able to install Gnome shell extensions manually. This can be great if you would not like all of the bloat that comes with installing a browser extension, but would still like to take advantage of the cusomization that Gnome shell extensions provide you. While this may not be the prefered method of installing shell extensions, but it is great to know if for some reason the browser extension doesn’t work or is acting buggy.
