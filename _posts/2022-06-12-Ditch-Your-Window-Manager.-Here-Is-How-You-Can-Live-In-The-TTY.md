--- 
published: true
---

A Linux users window manager, much like their text editor or browser, is a piece of software that they'll defend till their grave. There are hundreds of them, and each one comes with a different language, philosophy, and many unique features. And so many people are so busy arguing, many of them haven't considered, maybe it's better not to use any window manager at all? Depending on what you do with your computer, and your proficiency with the command line, it may be best for you to completely switch to using the TTY full time. In fact, I myself have been using the TTY exclusively, and have been having a great experience. So, to help you wayward souls who may be curious about a life without Xorg, I am going to explain some of the customizations that I've made, and how I overcome some of the challenges of living the terminal. 

# Making Everything Look Good

![TTY](/images/TTY.png)

I personally opted to use [Nord](https://github.com/lewisacidic/nord-tty), as it is the colorscheme that I am most familiar with. And as it turns out, theming the TTY itself is not hard at all. Just download the file, and put 'source FILENAME' in your .bashrc. 

And if you are going to use Tmux like me, I would recommend theming it too, as it makes your '*desktop*' look much more cohesive. It is a little more difficult to theme than the TTY, as you have to work with some plugins, but it is doable. If you want to use the Nord theme for Tmux, you can install it yourself right {here}(github.com/arcticicestudio/nord-tmux). 

# Making Tmux Usable

While Tmux is great, you have to do some configuring if you would like for it to look good and have some sensible keybindings. And since I personally didn't want to go through the work of configuring it myself, I took someone else's configuration. I know, it's cheap, but this configuration is really super easy to use and comfy. Especially as someone who uses Vim on the regular. It has Vim keybindings, an amazing status bar, improved pane maximizing, and much more. If you are interested, you can install it [here](https://github.com/pangliang/oh-my-tmux). 

# Multimedia 

## Watching Video 

The thing that I was the most concerned about, turned out to be extremely easy. For a while, I tried to get VLC to run in X without a window manager. But as it turns out, MPV has amazing support for Framebuffer. You just have to run MPV with these options to get it to run without X. 

  mpv --vo=drm FILE.FORMAT

## Viewing Images

This is another one that I was worried would not work. However, after doing some research, I stumbled on two image viewers that use Framebuffer, 'fim' and 'fbi'. These are both very similar, so whichever you would like to use is up to you, however I have had a better time with 'fim'. They support all major file types, including JPEG and PNG. They are also both very straightforward, and both work without any flags or configuration necessary. 

## Playing Music

Music is extremely easy to get running on a TTY, as there is no Framebuffer needed. I would recommend MPD+MPC, as it is one of the oldest, most reliable music players out there. I even wrote a blog about how to use it, and you can check it out right [here](https://thekernal.xyz/How-To-Use-MPD-And-MPC-As-Your-Music-Player/). 

# Using Xorg Apps

While most things can be done in the TTY, there are some exceptions. Graphic and Video editing is almost impossible. And while you can use a terminal based browser for a lot, interacting with the modern web is all but impossible without a graphical browser. But, as it turns out, you can still absolutely use some graphical apps without issue. Personally, the only GUI app that I use is Firefox, so I just have an alias for it in my ~/.bashrc. Here is the command that I use to launch it, and feel free to replace "firefox-esr" with anything you want. 

  xinit /usr/bin/firefox-esr $* -- :0 vt$XDG_VTNR" 

# Conclusion 

A life in a TTY is not for most people. It requires you to have a intimacy with the command line, do plenty of troubleshooting, and forces you to switch over to many TUI alternatives to all of your apps. However, if you're willing to put in the effort, and make some sacrifices, working entirely in the TTY may not just be possible, but could also be a very enjoying experience. And as an added benefit, if an amateur tries to break into your computer, they will have no idea what to do.
