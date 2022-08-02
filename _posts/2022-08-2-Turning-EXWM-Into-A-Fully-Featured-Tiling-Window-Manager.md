---
published: true
---
Emacs, for many people, is not simply an extensible text editor/Elisp interpreter. Emacs is a way of life. Many people who use Emacs prefer to never leave, and choose to use Emacs not only as their shell, text editor, file manager, but as their window manager as well. However, while EXWM is an amazing program, it doesn't result in a cohesive, attractive, or easy to use window manager. So, if you'd like to make your EXWM setup super usable with a custom modeline, wallpaper, and more powerful window management, here's some easy Emacs customizations to improve your EXWM experience.


<a id="orgec677f7"></a>

# Customizing The Modeline


<a id="orgf616f4c"></a>

## Adding Workspaces

If you use EXWM, workspaces are going to be how you move around with most of your graphical windows. But, by default, there's no way to find out what workspace you're on without pressing (s-w). Thankfully, like everything, there's a package to add it to the modeline. To install the package, you can just type,

	M-x package-install RET exwm-modeline

Then, once it's installed, you can either run it manually with `M-x RET exwm-modeline-mode`, or put

	(exwm-modeline-mode)

in your init file.


<a id="org85defd3"></a>

## Switching To Doom Modeline

While the default Emacs modeline is functional, it isn't the prettiest. To combat this, the community has made **many** different modelines. Doom modeline is the most popular of these endeavors, being used in Doom Emacs, Spacemacs, and Centaur Emacs, along with many people's personal configs. Follow the steps below to get Doom Modeline installed and in working order.

-   Add the [MELPA](https://melpa.org/#/getting-started) repository, using the instructions hyperlinked on this line.

-   Install '*doom-modeline*' and '*all-the-icons*' with the following commands. 
    
    	M-x package-install RET doom-modeline
    	M-x package-install RET all-the-icons

-   Put these lines in your Emacs init file.

		(require 'doom-modeline)
	
    	(doom-modeline-mode 1)
	
 		(require 'all-the-icons)


<a id="org679a6c4"></a>

## Moving The Modeline To The Top Of The Window

In most tiling window managers that come with a built in bar, the bar is placed at the top of the screen. This is a standard that many people expect. However, the default Emacs modeline at a first glance, appears to be locked in place. And while the modeline itself can't actually be moved, you can get the same result using something called a header line.


<a id="orgc98d722"></a>

### Enabling The Header Line, And Removing The Modeline (Mostly)

In order to do the brunt of the work, you can just move these lines to your Emacs init file.

	(setq-default mode-line-format nil)
	(setq-default header-line-format mode-line-format)


<a id="orgdcc9cd2"></a>

### Adding Hooks To Remove The Modeline On Certain Pesky Applications

While the previous lines of code are enough to remove the modeline on most applications, there appear to be a pesky few that continue to have both the modeline **and** the header line. To fix this, you'll need to install a package called 'hide-mode-line'.

	M-x package-install RET hide-mode-line

Then, start it in your Emacs init file.

	(require 'hide-mode-line)

In order to remove the modeline on your application of choice, you're going to need to add a hook. I'm not going to get into how hooks work in Elisp, but, I will provide you with an example. Here's the hook I added for 'emacs-dashboard' in my init file.

	(add-hook 'dashboard-mode-hook #'hide-mode-line-mode)

Feel free to exchange '`dashboard-mode-hook`' with any other application that is giving you trouble. 


<a id="org8afdbbe"></a>

# Window Management


<a id="orgfee13d2"></a>

## Ace Window

Ace Window is another quality of life application that's built in to almost every Emacs distribution, but the default GNU Emacs. Ace Window is a replacement for the default 'other-window', that attempts to make window management easier and more efficient, especially when it comes to a large amount of windows. When Invoked, Ace Window will assign each window a number, and allow you to choose which window you'd like to select just by typing the assigned number. You can install Ace Window like so. 

	M-x package-install RET ace-window

Then, you can bind it to 'M-o' by putting this line in your init file.

	(global-set-key (kbd "M-o") 'ace-window)


<a id="org7d932a1"></a>

## Wind move

If you'd like something a little more predictable and simple, you can instead choose Wind Move. Wind Move also ditches the default 'other-window', for a simpler and faster experience. With Wind Move enabled, you can move (Shift-ArrowKey) to move to the window up, down, left, and right of your current window. And since it's pre-installed, all you have to do is add these lines to your init file.

	(when (fboundp 'windmove-default-keybindings)
	(windmove-default-keybindings))


<a id="orgb1640d6"></a>

# Wallpaper

Due to the very nature of EXWM, and the fact that everything is running in Emacs, there isn't much reason to use a wallpaper. However, many people would prefer to have one. And while you can't have a wallpaper in the traditional sense, you can make Emacs transparent, in order to show a wallpaper faintly in the background of whatever Emacs buffer you're on.


<a id="org53dab39"></a>

## Installing The System Packages

Unlike all of the other improvements, you're going to have to install a few system packages. Depending on what disto you use, you can just copy-paste one of these commands.


<a id="orga75f80a"></a>

### Debian/Ubuntu

	sudo apt install feh picom


<a id="org5fc88f6"></a>

### Fedora/CentOS/RHEL

	sudo dnf install feh picom


<a id="org8dc363e"></a>

### Arch/Artix/Manjaro

	sudo pacman -S feh picom


<a id="org015d16f"></a>

## Acquiring Transparency On Emacs


<a id="org2848381"></a>

### Starting Picom

In order to get transparency, you're going to need to use Picom (or any other compatable compositor). If you start Emacs with your *.xinitrc*, you can simply put `compton &` in its own line, preferably before the `exec emacs` line.


<a id="orge6bd93d"></a>

### Enabling Compositing In Your Init File

While Picom will give you the ability to use transparency, nothing's going to happen unless you edit your Emacs init file. Move this little morsel of code into your init file to get 95% transparency. 

	(set-frame-parameter (selected-frame) 'alpha '(95))
	(add-to-list 'default-frame-alist '(alpha . (95)))


<a id="org70fbd3b"></a>

### Setting Your Background

While you're Emacs window is now transparent, there isn't a wallpaper to display. Just a black screen. To set the wallpaper, I recommend using Feh. Just put this line into your .xinitrc, preferably before the `exec emacs` line.

	feh --bg-scale /home/user/PATHTO/IMAGE.fmt


<a id="org8b5dba8"></a>

# Conclusion

While under no circumstances are all of these changes necessary, they will provide you with a much more usable, much easier to understand, and more powerful window manager from within Emacs. Many of the luxuries provided to you by more common tiling window managers will be provided just through these few customizations. And as an added benefit, you get to laugh at Doom Emacs users for having a bloated, inferior EXWM setup. 


# Table of Contents

1.  [Customizing The Modeline](#orgec677f7)
    1.  [Adding Workspaces](#orgf616f4c)
    2.  [Switching To Doom Modeline](#org85defd3)
    3.  [Moving The Modeline To The Top Of The Window](#org679a6c4)
        1.  [Enabling The Header Line, And Removing The Modeline (Mostly)](#orgc98d722)
        2.  [Adding Hooks To Remove The Modeline On Certain Pesky Applications](#orgdcc9cd2)
2.  [Window Management](#org8afdbbe)
    1.  [Ace Window](#orgfee13d2)
    2.  [Wind move](#org7d932a1)
3.  [Wallpaper](#orgb1640d6)
    1.  [Installing The System Packages](#org53dab39)
        1.  [Debian/Ubuntu](#orga75f80a)
        2.  [Fedora/CentOS/RHEL](#org5fc88f6)
        3.  [Arch/Artix/Manjaro](#org8dc363e)
    2.  [Acquiring Transparency On Emacs](#org015d16f)
        1.  [Starting Picom](#org2848381)
        2.  [Enabling Compositing In Your Init File](#orge6bd93d)
        3.  [Setting Your Background](#org70fbd3b)
4.  [Conclusion](#org8b5dba8)
