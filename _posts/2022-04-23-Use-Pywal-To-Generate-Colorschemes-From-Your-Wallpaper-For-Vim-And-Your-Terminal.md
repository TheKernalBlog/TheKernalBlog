---
published: true
---
Linux is, right now, the most customizable operating system on the market. It has hundreds of window managers, compositors, GTK themes, QT themes, Terminal emulators, and desktop environments. Yet, customization can be a little hard. It can often take hours, or even days to get everything set up how you like it. That doesn't have to be the case. Pywal is a super easy tool that allows you to  customize terminal color schemes, Vim, and various window managers. I am going to walk you through installing, getting, and applying a Pywal theme for your vim and your terminal emulator.

## Installing Pywal

Out of Ubuntu, Fedora, and Arch, Pywal is only available on Arch based distros through the community repository. So, if you are on an Arch based distro, use this command if you have the community repository enabled.

	sudo pacman -S python-pywal

But, if you are on Ubuntu, Debian, or Fedora, you can install it using these two commands.

### Ubuntu/Debian

	sudo apt install python3-pip

### Fedora

	sudo dnf install python3-pip

### Ubuntu/Debian and Fedora

	sudo pip3 install pywal

## Getting your theme

To get your Pywal theme, it is as simple as using this command, making sure to supply the path to the image.

	wal -i /PATH/TO/IMAGE

You should see that your terminal colorscheme change. But you will still need to apply it for it to work on your other terminals.

## Applying it

### Terminal

Terminals that use Xresources (xst, urxvt) should work out of the box, but other terminals will not work after the first time. If you use Konsole, Kitty, st, PuTTY, or Alacritty, you can go to [THIS](https://github.com/dylanaraps/pywal/wiki/Customization) link and learn how to apply them manually. But, if not, you can simply put this line in your .bashrc, .zshrc, or other startup file.

	(cat ~/.cache/wal/sequences &)

### Vim

Assuming that you have Vim Plug installed, you can add this line to your .vimrc, with the rest of your plugins.

	Plug 'dylanaraps/wal.vim'

Then, you just add this to the bottom of your .vimrc

	colorscheme wal

### Keeping the changes persistent

Unless you want the changes to only be temporary, you should add this line to your .xinitrc.

	wal -R

# Conclusion

If you would like to take a lot of the work out of having a stunning Linux desktop, Pywal is a great tool. It always seems to generate the best, most usable colorschemes from the most basic of wallpapers. It allows you to have a desktop on par with those Linux "Ricers", without having to look for a bunch of nieche themes from sketchy websites. And best of all, you don't have to use a wallpaper that matches your theme, even if it looks like crap.
