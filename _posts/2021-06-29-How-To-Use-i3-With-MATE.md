---
published: true
---
Lets admit it, i3 is pretty great. It provides a completely different work flow and look. The only problem is , you will probably have to configure it a lot. Some people don’t want to do that. You may be thinking, “What do I do then?”. It is simple. You use i3 with a desktop environment. I am going to go over how to use i3 with the “MATE” desktop environment. 

The first thing that you are going to have to do is make sure that you have dconf-editor. If you don’t use these commands to install it. 

Ubuntu/Debian: 

sudo apt-get install dconf-editor. 

Fedora/RedHat: 

sudo dnf install dconf-editor

Arch/Manjaro: 

sudo pacman -S dconf-editor

Now that you have that installed, make sure that you have i3 installed as well. Simply type these commands in the terminal. 

Ubuntu/Debian: 

sudo apt-get install i3 

Fedora/RedHat: 

sudo dnf install i3

Arch/Manjaro: 

sudo pacman -S i3

Now you get to the point where you can integrate i3 with MATE. You are going to have to follow this path in dconf-editor,  /org/mate/desktop/session/required-components/. You will see “dock, ‘Filemanager”, “panel”, and “windowmanager”. Make sure that you change “windowmanager” from default to “i3”. Then remove “filemanager”. You have to remove “filemanager”, because otherwise it will open a window in i3. 

You are now done! Simply log out or reboot into your desktop environment to see that it is now using i3 as a window manager. You can now enjoy the benefits of a tiling window manager without having to completely stop using a desktop environment.
