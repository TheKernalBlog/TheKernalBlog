---
published: true
---
Zsh is a fast, easy to use, and **extensible** shell for Linux and BSD based operating systems. And while yes, being fast and easy to use are very important qualities in a shell, most
people switch to Zsh because of how darn customizable it is. There are hundreds of useful plugins and beautiful themes that you can install without breaking a sweat. So, if you use Zsh,
and would like to improve your workflow with a couple super-useful plugins, I have compiled 5 of my personal favorites that will work on any operating system. 


<a id="org0361a7f"></a>

# [zsh-interactive-cd](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/zsh-interactive-cd)

After getting really used to similar functionality in Eshell, I found this plugin extremely useful. When using cd, if you enter something that isn't a complete directory, and you hit
*TAB*, a menu will pop up, listing all of the current directories that you can cd into. Then, you can make use of the arrow keys to select a directory and enter it. This is especially
useful for when you are working with a large amount of directories and can't be expected to remember them all or use the traditional *TAB* autocomplete. It is really just a small quality
of life change that makes the command line a little more tolerable, for when you can't be expected to use a file manager.

![ZSHCDPLUGIN](/images/zshcd.png)

<a id="orgf12962f"></a>

# [vi-mode](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/vi-mode)

Bash's built in vi mode is extremely useful for people who spend the majority of their time using Vim and Vim like applications. So it only makes sense that people would like to bring
that same functionality to ZSH. I have to say, after messing around with vi-mode on ZSH, and doing some basic commands, I found the experience near;y identical to Bash's vi mode. You have the
basic 'input' 'visual' and 'normal' modes, along with Vi keybindings for moving around and editing. There really is no better feeling than moving around with hjkl, switching modes, and
using all of the fancy Vi commands without even having to launch Vim. 


<a id="org4018a8e"></a>

# [thefuck](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/thefuck)

The name aside, this is an extremely useful plugin that saves a lot of time. Just by double-clicking  *esc*, 'thefuck' will attempt to find the error in your command, and correct it for
automatically. For example,

if I were to type,

`sudo aot update`

then 'thefuck' will find the spelling mistake and fix it for me.

`sudo apt update`

Think of it like spellcheck, but instead of correcting a simple <del>wird</del> **word**, it can correct your whole command. 


<a id="org0e51150"></a>

# [extract](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/extract)

Extracting files from the terminal is extremely complicated, especially when compared to extracting files in a file manager. You have to remember what command to use for every binary,
zip file, tar file, and all 10,000 other types of archives. But thankfully, there is a silver bullet for every type of archive. 'extract' will extract almost any file you can think of.
It's as simple as running

`extract file.type`

You don't even need to specify what file type the file is, just run 'extract' and it will do the rest. 


<a id="org6f19f26"></a>

# [aliases](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/aliases)

Aliasing common commands is something that saves a lot of time. But, personally, I have a hard time remembering all of the aliases that I've set. And it's really frustrating when you
**know** that you have an alias for something, but can't remember what it is. But with this plugin, all you have to do is type `acs`, and all of your aliases will be laid out in front of
you. You can even search using `acs 'KEYWORD'`, and it will show you a list of all your aliases associated with that keyword. You should really consider installing this one if you
are as forgetful as me. 

![ZSHALIASPLUGIN](/images/zshalias.png)


<a id="orgfaacd63"></a>

# Conclusion

These 5 plugins provide a faster, more efficient way to use your shell while being OS agnostic and super easy to use. They allow you to extend your shell in a useful way, without bloating
your shell to the point that it gets a stomach ache. Install all of the plugins, try them out, and if you aren't a fan, you're only a # away from getting rid of them. 


# Table of Contents

1.  [zsh-interactive-cd](#org0361a7f)
2.  [vi-mode](#orgf12962f)
3.  [thefuck](#org4018a8e)
4.  [extract](#org0e51150)
5.  [aliases](#org6f19f26)
6.  [Conclusion](#orgfaacd63)
