---
published: true
---
Desktop environment hopping is something that many novice and experienced Linux users do for fun. Some days you may feel like using GNOME, KDE, XFCE, or another desktop. And Red Hat based systems, have an excellent way of installing and removing desktop environments. Using the dnf package manager, I am going to show you how to remove your previous desktop, and install another one.

# Finding the group names of the two desktop environments 

All of the desktop environments in RHEL based systems are organized into groups. To find the group name of your desktop environment, you can type this command in the terminal.

        sudo dnf grouplist -v

This will list all of the groups available. But to start, you should look for the "Installed Groups" section. Here, you should see your desktop environment. In my case, it is "(xfce-desktop) but it will likely be something else depending on your desktop environment. You also need to find the group name for the new desktop environment you would like to install, in my example, "(kde-desktop-environment)".

# Removing your desktop environment 

Now is the big scary part of the process. You are going to remove the desktop environment completely, and kick yourself back to the terminal. But don't worry, it really is not hard to get your GUI back. To remove your desktop simply type this command, making sure to replace the default text with whatever group name your desktop environment has.

        sudo dnf remove @Desktop-Environment-Here

Your entire desktop will be snapped out of existance. So it is time to get a different desktop back.
 
# Installing your new desktop environment 
 
To install your new desktop, it is literally just the opposite step that you need for removing your desktop. Simply type this command in your terminal and, much like last time, replace the de
fault text with the new desktop that you would like to install.

        sudo dnf install @Desktop-Environment-Here

# Switching to the new desktop environment 

You are almost there. All that you need to do now it set up the display manager. One super easy way to do this is switchdesk. You can install switchdesk using dnf with this one command.

        sudo dnf install switchdesk

Now, all that is required to do is type "switchdesk" followed by the name of your new desktop environment. One example is this.

        sudo switchdesk XFCE

# Conclusion 

I have changed my desktop environment too many times to count. With Fedora, Rocky Linux, or CentOS you can use dnf groups to change up your desktop easily in around 10 minutes without any iss
ues. Because, sometimes, you need to switch things up, and a new desktop environment is a great way to do that. So, if you feel like you need a new look, give it a try. Nothing bad is going t
o happen.
