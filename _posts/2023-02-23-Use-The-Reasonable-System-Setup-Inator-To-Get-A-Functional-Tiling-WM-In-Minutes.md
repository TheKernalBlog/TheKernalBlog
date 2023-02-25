---
published: true
---

![IMG1](/images/DesktopRSII.png) 

I'm definitely not the first person to do this. In fact, I've made use of many similar shell scripts & configurations in the past. But, still, I believe that RSII in particular provides a lot. It's significantly less colorful, flashy, or complicated as other scripts; that's by design. RSII, is a very bare bones i3 & Vim configuration that you can plug & play on any distro without needing much prior experience. So, if you think that sounds like something you'd be interested in, get ready. Because I'm going to show you how you can download and run my RSII, and get everything up and running in under 10 minutes.

# Downloading The Script 

## Installing Git 

Before you can download RSII.sh, you'll need to have *git* installed. In most cases, it will be installed on your system. But, if it's not, feel free to copy one of these commands into your terminal. 

### Ubuntu 

    sudo apt install git 

### Fedora 

    sudo dnf install git 

### Arch 

    sudo pacman -S git 

## Downloading & Moving script 

To download RSII.sh and move it into your home directory, you can copy this command into your terminal. 

    git clone https://TheKernalBlog/RSII/ && mv ~/RSII/RSII.sh ~/ 

Then, make it executable. 

    sudo chmod +x ~/RSII.sh 

# Running the Shell script

![IMG2](/images/ScriptRSII.png)

Now it's time to start the shell script! You can run the shell script like this, making sure not to use sudo.  

    ./RSII.sh

## Distro 

First, you'll be asked: 

    What distro are you using: Ubuntu, Fedora, or Arch (U/F/A) 

Use one of the three letters to select your distro, then hit enter. After you've done that, all necessary packages will be installed, so be prepared to wait. 

Once all the packages are installed, the RSII directory will be cloned from github, and all pertinent files will be moved to their respective places.

## Monitors 
![IMG3](/images/Monitor15.png)

Now, you'll be asked: 

    Would you like to use a GUI to configure multiple monitors? (y/n) 

If you're in a TTY, or only have one monitor, type *n* and move on. But, if you do have multiple monitors, type *y* to bring up arandr. 

Here, you can use arandr to move around, flip, and mess with your monitors to your hearts content. Then, once you're ready, follow the instructions. Click *save as*, and save your configuration in the pre-programmed directory as *monitor.sh*.  

And once you're ready to move on, type *y* and you'll be taken to the next section. 

## Vim 

![IMG4](/images/VimRSII.png) 

Here, you don't have to anything. Just sit back as Vim pops up and installs all the best plugins for you. 

## Guide  

![IMG5](/images/GuideRSII.png) 

Finally, you'll be met with one final prompt. It will ask: 

    Are you currently using a GUI? (y/n) 

If you answered yes, Zathura will pop up with with the guide. It's incredibly simplistic, so just spend a minute reading over the keybindings before log in to RSII. 

# You did it! 

If you followed all the instructions laid out in the shell script and in this blog, you should now have a working i3 setup with a newfangled Vim configuration. It's not the most awe-inspiring configuration available, but if all you want is a nice distraction free environment with an efficient workflow, you've got it. Sure, you could use LARBS or Archrice, but I think there's definitely a reasonable argument for using RSII instead. And while I may have used analogous scripts in the past, here's hoping that this is the last one I ever try. 
