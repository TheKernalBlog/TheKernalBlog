---
published: true
---
Linux, unlike what some people think, has pretty great app support. However, there are still some applications that will only run on windows. This can actually run these apps on linux using Wine. Wine stands for, “Wine Is Not a Emulator”. It allows you to run .exe files on Linux. I am going to go over how you can install, run, and use Wine to use Windows programs on Linux. 

The first thing that you are obviously going to have to do is install wine. This can be achieved by typing these commands in the terminal based on what distro that you use. 

Ubuntu/Debian: 

	sudo apt-get install wine

Arch/Manjaro:

	sudo pacman -S wine 

Feora/RHEL: 

	sudo dnf install wine 

OpenSUSE: 

	sudo zypper install wine 

You will need to enable 32 bit architecture. You will probably have to do thisyou have a computer that was made in the past 10 years. Type this in your linux terminal to achieve that. 

	sudo dpkg --add-architecture i386

Now that you have it installed, you are going to have to configure wine so that it will actually work. Wine is going to have to make a home “windows” drive. This can be done by typing this in the terminal. 

	Winecfg

You will see that this makes a windows folder in your home directory. In the window that opens, you can choose your windows version. I use Windows 7, but you can use something else if you would like so. Click “apply” and then you can close the window. 

You are almost done. Now all that you need to do is find the .exe file that you want to use. Right click it, and then open the dialogue that says, “run with” and click “Open With Wine Windows Program Loader”. Now it will install, and it will be put in your application menu. 

You now can run that program from your application menu. You will be able to run some Windows programs with Wine. This works for some games, and simple applications. Now you will not be held back from Linux because there are some applications that you need that only work on windows.
