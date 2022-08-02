---
published: true
---
/home/ is a sacred place. It should have your unhidden directories, and a few hidden ones for things like .local or .config. Yet, now it seems like every single app now adds a useless hidden file that could have easily been in .config. So, I am going to show you where you can put some of the files clogging up your /home/ directory, and even some alternatives that don't require a file in /home/.

## Moving some files.

Xorg adds some useless files right in your home directory. Your .xinitrc, .xprofile, and .Xresources file don't actually have to be in /home/. You can put them in your .config directory with these commands.

	mkdir ~/.config/x11

	mv .xinitrc ~/.config/x11/xinitrc

	mv .xprofile ~/.config/x11/xprofile

	mv .Xresources ~/.config/x11/xresources

The same can be said with Zsh and the .zshrc file. In a very similar fashion, you can move it like so.

	mkdir ~/.config/zsh

	mv .zshrc ~/.config/zsh

And then, you can move your .vimrc into a init.vim file in your .config directory with these commands.

	mkdir ~/.config/vim

	mv .vimrc ~/.config/vim/init.vim

All of these places in .config will get you the full functionallity that you would get if they were in your /home/ directory without having the huge eyesore whenever you type 'ls -a'.

## What not to use

While I covered a few of the most basic programs where you can move their config files to a more sensible place, it is with great sadness that I tell you, some of the most essential programs on Linux don't actually have any path where you can move them out of your home directory. Yet, they have alternatives. So I will offer some alternatives if you are really serious about having an uncluttered /home/.

### Browsers

Both Firefox and Chromium based browsers leave a useless .mozilla and .pki directory respectively. This includes .librewolf and even some WebKitGTK based browsers like .surf. But there are some exceptions. Ungoogled-Chromium doesn't leave a .pki directory, and KDE's Falkon browser only has a ~/.config/falkon directory.

### Shell

Bash, Ksh, and many other shells require a file along the likes of .bashrc or .kshrc. But, the two other most popular shells can use a propper config file in your .config directory. If you are stupid enough to use Fish, or decide to use ZSH, you can put them in your ~/.config/fish and ~/.config/zsh files instead of your home directory.

# Conclusion

.config for config files, data in .local, and temporary files in .cache. That's how it's been for a .long time, and there is no reason to change it. Not only does it make your /home/ directory less cluttered, it makes it easier to find all of the files that you will need, instead of them being in a big ol' melting pot. Plus, you can brag when you run 'ls -a', and laugh at the people with 40+ files.
