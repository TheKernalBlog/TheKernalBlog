---
published: true
---
I am a big fan of using a Window manager instead of a desktop environment. They are lightweight, and super customizable. The window manager that I use is Openbox. It is a little harder to configure than i3, but it is still fairly easy to customize. I am going to go over how you can not only launch applications on the startup of Openbox, but create keyboard shortcuts to launch an application.

# Autostarting Applications

This is a very simple process. All that you have to do is make the autostart file, and add any applications that you want to autostart. You are going to have to cd into the openbox directory. Make sure to go to .config/Openbox. Then use the touch command to make a file called “autostart”. Open it up with your text editor of choice, and use these commands for the applications that you want to autostart. 

Regulat autostart:

	NAMEOFAPPLICATION &

Autostart with restore:

	NAMEOFAPPLICATION –restore &

This can allow you to use external applications to set your wallpaper, enable compositing, and add a panel. If you are using Openbox for a long period of time, you are defiantly going to use this file a lot. 

# Adding Keybinds 

While most people can very easily use the autostart feature, a lot of people struggle with adding keybinds, It is not as simple of a process. You are going to have to go to the rc.xml file and make your own code. Again, you are going to have to .config/openbox , and then open the rc.xml file and add these lines of code under the keyboard section. Here is an example of what it would look like. 

	<keybind key =”Key-Key”> <action name=”execute”> <command>THEAPP </command> </action> </keybind> 

If you would like to see a more realistic example, here is my config that launches Rofi when you type Super+d. 

	<keybind key="W-d"> <action name="execute"> <command>rofi -show run </command> </action> </keybind>


# Conclusion 

You now know how you can not only start an application on startup, but run an app using a keybind This should help you in being able to use the Openbox Window manager as a full desktop. Now you can effortlessly run any applications that you need without having to launch it manually, or by opening the Openbox menu,
