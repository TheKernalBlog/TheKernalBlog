---
published: true
---
Snaps, oh snaps, the bane of Ubuntu. If there is one criticism to be leveraged at Ubuntu, it is their snap packaging system. Much like AppImage and Flatpak, Snaps consist of one single package that is isolated from the rest of the system, and includes all of the dependencies. The problem arises when these snap packages start to take up more space and open slower. So, I, like many Ubuntu users am going to show you how you can remove snapd, and everything related to it.

# Removing all snaps 

Before it is safe to remove snap, it is recommended that you use snap to uninstall all of the snap packages already installed on your system. You can show all of the snap packages installed using this one command.

        snap list

Now that you know all of the snaps that are on your system, you can remove them with this command.

        snap remove PACKAGENAME


# Clearing the snap cache 

Before you completely uninstall snap, it is always a good thing to clear the cache so that there isn't just some unneeded cache on your system. You can achieve this with this command.

	sudo rm -rf /var/cache/snapd/

# Removing snaps 

You are now ready to uninstall snap itself. Make sure to do this with this command so that you can completely remove it and all of it's configuration files.

        sudo apt purge --autoremove snapd

# Removing the snap directory 

Snap is very annoying as it leaves a 'snap' directory chilling in your home directory that holds all of your snap packages. Now that the actual snap daemon is removed, you should be safe to remove the directory. You could either do it graphically with your File manager, or just use this command.

	rm -rf ~/snap

# Holding the snap package 

You will notice that if you try to install, for example, Chromium with apt, it will just prompt you to install snap again. This is why you need to, 'hold' snap. This makes it so that snap cannot be installed, updated, or removed, so it is important that you do this last. You can hold snap by typing this command in the terminal.

	sudo apt-mark hold snapd

# Conclusion 

While there are some people who like Snaps, many don't, and by following these few commands you can remove snap from Ubuntu, so that you can continue to enjoy your stable server and your new shiny desktop without being worried about snap packages slowing you down and taking up all of your disk space.
