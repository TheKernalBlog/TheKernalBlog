---
published: true
---
Currently gaming on Linux is great. You have a lot of support from major developers and due to the fact that Linux is faster, you will most likely get better and more stable frame rates when gaming on old machines. However, especially with indie games, you won’t be able to play them on Linux by usual means. This is why I am going to walk you through how you can take the .exe file for a Windows game and use Lutris to play it. 

# Download Lutris 

Obviously to run games with Lutris, you are going to need Lutris installed. Installing Lutris will also install Wine and potentially some drivers that Lutris needs. Depending on your distro, just copy-paste these commands into the terminal. 

## Ubuntu/Debian based
	sudo apt install lutris 

## Arch based 
	sudo pacman -S lutris 

## Fedora 
	sudo dnf install lutris

## OpenSUSE
	sudo zypper install lutris

# Setup Wine 

In your terminal run the ‘winecfg’ command. This will set up a virtual C: drive in your .wine directory. It will ask you what version of Windows you would like to use, I would prefer to use Windows 10 as it allows you to get the most app support. 

# Setup everything for the installation 

If it has not been done already, make a file called ‘Games’ in your home directory. If you have a file that contains the .exe file, move it there. If you just have the .exe file, put it in a folder with the name of the game, and then move it to the Games directory. 

# Install from within Lutris. 

Finally, it is time to open Lutris. Once you open it, click on the plus button to add a name. Here you can add the name of the game along with the date is was released if you so please. Under the section that says ‘Runner’ select Wine. Under ‘Executable’, click the browse button and select the .exe file from the file that is in the games directory. Then, under ‘Working directory’ select the folder where the .exe file is contained. 

# Conclusion 

Now you should be able to select and play the game from Lutris without any hassle. This is super convenient so that I can still play all of my favorite Windows games without having to open up the file manager or terminal and open it up with Wine manually. 
If you would like to see the official websites of Lutris and Wine, here they are. 

Lutris: [Click Me!](https://lutris.net/)

Wine: [Click Me!](https://www.winehq.org/)
