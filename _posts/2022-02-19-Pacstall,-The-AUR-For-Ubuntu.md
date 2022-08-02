---
published: true
---
If you were to ask an Arch user why they use Arch Linux, one of the most popular responses would be, "I love the AUR". It's true, the AUR is an amazing tool that allows you to install almost anything that you could ever dream of, which is why it makes sense that people would like to have an equivalent on another distribution. Pacstall is the AUR for Ubuntu, and it is growing fast. So, if you use Ubuntu and would like to show off to Arch users, I am going to show you how to install Pacstall and use it to install and uninstall packages.

# Installing

Thankfully, instead of having to build it from source, Pacstall has a nice bash script that you can use to install it. However, you need to make sure that you have the dependencies installed beforehand, and you can install them with this command.

	sudo apt install wget curl

Then, you can install using the bash script like so.

	sudo bash -c "$(curl -fsSL https://git.io/JsADh || wget -q https://git.io/JsADh -O -)"

# Using Pacstall

Now that you have it installed, you will find that despite being a recreation of the AUR on Ubuntu, it does not act like the package manager for either Arch or Ubuntu. So if you would like to install, remove, update, or search for software with Pacstall, I am going to show you all of the commands.

## Installing Software

	pacstall -I PACKAGENAME

## Removing Software

	pacstall -R PACKAGENAME

## Searching Software

	pacstall -S PACKAGENAME

## Updating software

	pacstall -Up

# Conclusion

While it is still in its infancy, Pacstall is a great tool and something that will inevitably gain more packages and more utility.  While it already has some great packages, (Brave, Librewolf, AppimageLauncher, and nala) it is only going to get more. It will allow you to get some of the packages not in the official repositories without having to use Snap or Flatpak. So try it out, and feel the power of a user repository.
