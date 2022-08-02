---
published: true
---
Emacs is often confused for a text editor. While Emacs has a text editor, at its core, Emacs is a Elisp interpreter. Because of this, Emacs is very extensible. For example, I use it as my web browser, file
manager, agenda, text editor, and now, my window manager. You may be pleasantly surprised to find out that through EXWM, Emacs can be used as your window manager. If you would like to use EXWM, I am going to
go step-by-stop on how to get EXWM to work, but you can fiddle with and learn how to use it yourself.

## Installing the EXWM package.

This guide is going to assume that you are using GNU Emacs, but the same will apply on other distributions of Emacs, with the exception of some keybindings. So, while you might rush to your package manager and
try to install it that way, you can actually install EXWM through Emacs itself. Just type M-x and then enter, "package-install". This will prompt you for what you would like to install, and from there you can
simply type "EXWM". Then, after a minute or two of waiting, you should be able to restart Emacs and realize that EXWM is installed.

## Enabling EXWM

Here is where you are going to have to edit your config file. But don't worry, you don't actually have to know any Elisp. If you would just like a basic EXWM config that doesn't have anything flashy or extra,
you can copy and paste these lines of code into your ~/.emacs.d/config.el.

    (require 'exwm)
    (require 'exwm-config)
    (exwm-config-default)
    (require 'exwm-systemtray)
    (exwm-systemtray-enable)

## Configuring Multi-Monitors

If you are on a laptop, or only have one monitor, you can skip this section. While many people would say that you should configure exwm-randr in the config file, I would recommend against that. What I personally
do, and what I would recommend you do, is write a bash script and put it in your .xinitrc. While you may be saying, "But I don't know how to script in Bash", you don't have to. Making use of 'Arandr', you can use
a GUI to configure your monitors, and you will have a bash script generated for you. Then, in your .xinitrc, at the top of the file, you can simply write the path to the bash script and your monitors will be
configured.

## Starting EXWM

Starting EXWM is simple, especially if you are not using a display manager. So, for the purposes of this guide, I am going to recommend removing your display manager. If you don't know how, and your distro uses systemd, you can disable it like so.

         sudo systemctl disable DISPLAYMANAGERHERE

Then, it is time to edit your .xinitrc. If there is anything already there that starts with 'exec', comment it out or delete it. Then, you just have to type 'exec emacs'. This will mean that when you start xorg,
it will launch Emacs. Finally, you can start Xorg with the "startx" command. It will launch Emacs, and by extension, EXWM.

# You're Done!

If you have followed this guide, you can now launch Emacs with EXWM. While there is still lots to learn with EXWM, it is great for your productivity, and allows you to become even better with Emacs. At the very
least, it is quite the brag to say that Emacs is your window manager.
