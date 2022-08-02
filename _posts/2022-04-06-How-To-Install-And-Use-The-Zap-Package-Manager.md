---
published: true
---
AppImage, while being one of the oldest, fastest, and easiest universal package formats, it's not nearly used as much as Flatpak or Snap. One of the main reasons that people decide
to put off AppImages is the fact that, there isn't a regular, CLI package manager. While that used to be the case, there is actually a new package manager out that allows you
to speedily and easily install almost all AppImages. I am going to show you how you can prepare, run, and install the Zap package manager on every Linux distro. 

## Installing all the dependencies 

Before you install Zap, you are going to need to get some dependencies. Many of these packages are pre-installed on many distros, but, to be on the safe side, you can install them.
Depending on what Linux distro you use, you can do so with one of these commands.  

### Ubunu/Debian

	sudo apt install curl grep jq wget

### Fedora/CentOS/Rocky

	sudo dnf install curl grep jq wget

### Arch/Manjaro 

	sudo pacman -S curl grep jq wget

### OpenSUSE

	sudo zypper install curl grep jq wget

## Installing Zap 

While you can manually install Zap, and the instructions to do so are on their github page right [here](https://github.com/srevinsaju/zap), it is much easier to install Zap with their handy little Bash script. If you 
would like to do so, you can just copy-paste this command into your terminal. 

	curl https://raw.githubusercontent.com/srevinsaju/zap/main/install.sh | bash -s

This command will install Zap locally in .local/bin, but if you would like to install Zap system-wide, you can just add 'sudo' before the 'bash -s'. 

## Using Zap 

In terms of usage Zap is not that different from your traditional package manager. Most of the commands that you would expect are there, and even some you wouldn't expect. 
For example, 
### Installing software

	zap install PACKAGENAME

### Updating software 

	zap update PACKAGENAME 

or 

	zap upgrade

to update all packages. 

## Configuring Zap 

	zap init

This will bring up a graphical TUI interface that will allow you to configure the behavior or zap. 

## Running the Zap daemon 

	zap daemon --install

This is similar to snapd, in the way that it will run a local Systemd service that will automatically update all of your AppImages for you. 

# Conclusion 

Zap is an amazing package manager that fills a gap we've needed to be filled for a long time. As a easy to use, easy to understand, and feature rich AppImage package manager, it makes 
ditching Flatpak seem like a much easier and better option. You won't have to worry about the wims of Cannonical or Red Hat, and you can use the independent, speedy, and 
decentralized AppImage format without having to do all of the dirty work yourself.
