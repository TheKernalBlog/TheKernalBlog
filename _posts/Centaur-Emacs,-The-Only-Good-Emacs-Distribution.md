---
'0': p
'1': u
'2': b
'3': l
'4': i
'5': s
'6': h
'7': e
'8': d
'9': ':'
'10': t
'11': r
'12': u
'13': e
published: true
---

No matter how much your try to fight it, you always come back to Emacs. It is not only an amazing text editor, but an amazing file manager, window manager, shell, and even browser. I personally have switched back to Emacs, as its productivity features and extensions geared towards writers are just unrivaled. However, I am not a fan of Doom Emacs. And I don't want to spend 10+ hours perfecting my Emacs config. So, I set out on a quest, to find the Emacs distribution that fits my every need. And after around 20 minutes of digging, I found the perfect mix of vanilla Emacs, eye candy, and extra features. For me, that is Centaur Emacs. Centaur Emacs is a super easy, snappy, and configureable Emacs that doesn't rock the boat too much. And since I have been spending so much time with it recently, I thought it fair to share my experience with you, and hopefully get your attention on this amazing Emacs distribution.

# Instillation

The install for Centaur Emacs is one of the more straightforward than many of the others that I've done. There is no options while installing, no splash screen, no progress bar, you just copy the files to your *~/.emacs.d* and then open Emacs and wait 2-5 minutes for all of the packages to install. In fact, if you already have Emacs installed, you only need two commands.

## Getting *~/.emacs.d* out of the way

### Creating A Backup

    mv ~/.emacs.d ~/.emacs.d.bakup

### Deleting It Entirely

    rm -Rf ~/.emacs.d

## Cloning The Github Repository

git clone https://github.com/seagle0128/.emacs.d ~/.emacs.d

# Speed

My specs are as follows.

### CPU
> Intel i5, 8 Core CPU

### RAM
> 8 GB

### GPU
> Intel WhiskeyLake UHD Graphics

So far, Centaur Emacs has been running as smooth as silk. I have had no freezes at all, and have consistently stayed under 10% CPU usage and 500MB of RAM usage on Ubuntu with EXWM running. In terms of boot speed, Centaur Emacs hovers around 3-5 seconds. Which, while not terrible is slower than default Emacs. But, if that's really a huge problem for you, consider [running Emacs as a daemon](https://emacswiki.org/emacs/EmacsAsDaemon).

# Appearance

![LookingGood](/images/CentaurMacs.png)

Centaur, in terms of appearance, is very comparable to Doom Emacs. However, there are some small differences. For example,  Centaur uses 'doom-themes', but handles theming differently. Just run 'centaur-load-theme', and pick between one of the 8 options. But of course, you can always do the dirty work yourself and edit the *~/.emacs.d/custom.el* yourself. There is also a custom configuration of the status bar, which looks great and is very light one resources. Centaur Emacs even comes with a super nice, custom dashboard that is chocked full of featres, and is configurable to your hearts content.

# Configuration

Centaur Emacs can be configured in the exactly same manner as regular Emacs. There is no seperate directory where you have to run a command to update your configuration. Just go to your *~/.emacs.d* and configure the exact same file that you would on regular Emacs. And thankfully, Unlike Doom Emacs, there isn't another package manager, so you can just run 'package-install' and restart Emacs to install any plugin you could ever need.

# Nifty Apps

### Org-Agenda

Org-Agenda is the sole reason that some people use Emacs, it's just that good. You can make an Org file that can include your tasks, notes, due dates, and much more, and then have it neatly displayed as an agenda. You can just put 'Agenda.org' in your */org* directory and use it immediately.

### Vterm

I absolutely love Eshell, and tolerate the defualt 'ansi-term', but sometimes you need something a little more powerful. And Vterm does that better than anything else. Vterm loads fast, uses your default shell, and is packed full of features that aren't in 'ansi-term'. There really is no reason not to use it.

### Treemacs

If you use Vim or VSCodium, there is a good chance that you have a file tree on the left of your editor. And if you are missing this crucial feature, you can just use the keybinding 'C-x t t' to launch the file tree. From there, you can navigate the current directory and select the file to do with what your please.

### Ace window

When you press 'C-x o' to switch windows in Centaur Emacs, you will notice something out of the norm. You are prompted to press a number in order to select the window that you would like to switch to. This saves a lot of effort, since you don't have to press 'C-x o' 20 times just to get to your preferred window.

### Counsel

In the same vein as Ace window, Counsel is a replacement for the regular 'M-x' menu. Thankfully, it doesn't change a whole lot. The menu looks a lot like Rofi, spawining in the middle of the screen and boasting predictive auto-complete. It even has the ability to study the keybindings for any application on demand. Other than that, it acts just like the standard 'M-x' menu.

# Conclusion

Centaur Emacs may not be the best Emacs distribution for you. If you are not already familiar with Emacs, it can get a little complicated, and it is less intuitive to configure and install. However, I truly believe that for a large amount of the people readingf this rightf now, Centaur Emacs may be just what you need. It is fast beautiful, and super friendly for the power-user. Leave the world of [evil](https://github.com/emacs-evil/evil), and be free.

### Install Here

![Logo](/images/logo.png)

[Click Me!!](https://github.com/seagle0128/.emacs.d)
