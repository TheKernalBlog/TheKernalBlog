---
published: true
---
I have been trying out Pop OS 21.04, and one of the main things that made me switch is Cosmic. Like many other desktop environments, Cosmic was made to battle the shortcomings of Gnome. This feature packed desktop has an amazing workflow and defaults. I am going to explain why Cosmic caught my eye, and how you can install it. 

# Separation 

If you have used Gnome, you will know that by hitting the super key you have access to a app overview, your opened windows, your workspaces, and even the ability to search for files. Cosmic, tries to differentiate itself from Gnome by separating all of these. There is a different combination of keys/buttons on the panel for 3 elements. There is a window overview that allows you to switch workspaces, a application launcher that is a lot like Gnome’s, then there is a Rofi like menu that not only allows you to launch applications, but switch between open windows too. 

# Keyboard Shortcuts 

Much like Gnome, Cosmic comes packed full of keyboard shortcuts. Opening the web browser, file manager, terminal, is all pre-configured to open up with a simple keyboard shortcut. You can also switch windows using the arrow keys. Then, best of all, by pressing Super+Enter you can enter a mode where you can move and resize a window around using the arrow keys. Much like Gnome you can also switch workspaces with a keyboard shortcut. Plus, if you forget any of the shortcuts, the widget on the top panel allows you to show a window that has all of the shortcuts laid out for you. 

# Trackpad gestures 

I use a laptop, and by extension use the trackpad a lot. The gestures that Cosmic uses are just so great. I can switch windows by swiping up and down with 3 fingers, I can show the applications view by swiping right with 4 fingers, I can show the window overview and workspace switcher by swiping left with 4 fingers, and I can switch workspaces by swiping up and down with 4 fingers. These are all super intuitive and easy to learn gestures that I find myself using a lot. For what I connect my laptop to my external monitor, I have even considered buying a trackpad to use instead of a mouse because the gestures are just that great. 

# Tiling Windows 

This is one of the main reasons that people switch over to cosmic. It allows you to switch between floating and tiling windows on a dime. While tiling, you can choose gaps, the color of the window titles, and even choose applications that will be floating even in tiling mode. It is the only desktop that is not only user friendly, but allows for you to tile windows. I have found it to really boost my workflow, as I can have all of my windows open and on screen at all times. 

# Installation 

You may be thinking, “That sounds great, but how do I install it”. Fear no more, as is is super easy to build from source. Assuming that you have Gnome already installed, just copy-paste these 3 commands into your terminal. 

	git clone https://github.com/pop-os/cosmic

	cd cosmic

	make && make install 

Then as outlined in <a href="https://github.com/pop-os/cosmic">The Github Page</a> 
 , in Gnome extensions, you will need to install enable the “Ubuntu Dock”, “Pop COSMIC”, and “Multi-Monitors Add On”. 

# Conclusion 

Cosmic is a amazing desktop, and I applaud the PopOS team for all of the work that was put into this amazing desktop environment. It really feels like a upgraded gnome. This is the most productive and amazing desktop that I have ever used, and I would recommend that anyone who is interested to try it out.
