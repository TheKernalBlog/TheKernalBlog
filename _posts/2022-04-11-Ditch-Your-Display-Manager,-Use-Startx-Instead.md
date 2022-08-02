---
published: true
---
When you boot into your Linux desktop, what do you see? If you are using the desktop version of most Linux distros, such as Debian, Fedora, or Ubuntu, you are going to see a display manager,
or, more commonly referred to as a "login manager". While these have a use, especially if you are someone who has multiple graphical interfaces that you switch through on a regular basis,
for many people, they may as well be useless. So, if you would like to skip the hassle, and get right into your X session as fast as possible without any fancy GUI, I will show you how to
remove your login manager, edit your .xinitrc, and then start Xorg.

## Removing Your Display Manager

To get rid of your display manager, you first need to know what display manager you are using. In most cases, you can easily find out by simply knowing what desktop environment you are
using. For example, if you use GNOME, you are probobly using GDM as your display manager. If you really don't know, the best way to find out is to compare what your login screen looks like
compared to what the display managers look on one of the many listicle websites showcasing display managers.

Then, once you know what the name of your display manager is, you can disable it on startup like so.

        sudo systemctl disable DISPLAYMANAGER

## Creating Your .xinitrc File

If it is not already there, you can just create the file like so.

        touch .xinitrc

Then, open it.

        TEXTEDITOR .xinitrc

Once you have it open, you will have to put a line that says, "exec", followed by your desktop environment. If you are a little confused, here is a list of what you have to put after the
"exec" depending on what desktop environment you use.

+ GNOME - gnome-session
+ KDE - startkde
+ XFCE - startxfce4
+ MATE - mate-session
+ LXQT - startlxqt

If you are using another desktop environment, or a minimal window manage, it is either in the manpage of the desktop/wm or on their website.

## Starting Xorg

Then, to actually boot into your desktop, you simply type

        startx

into your shell with no other graphical interface running, and you will boot into your DE or WM.

# You Did It!

If you followed all of my instructions, you can now simply type 'startx' into your shell and have your GUI run. It is not only much faster, but it is extremely convenient to simply be able to
type 'startx' without having to worry about setting up and maintaining your display manager. Plus, it looks a lot cooler to launch your GUI from the terminal than having a regular login
screen.
