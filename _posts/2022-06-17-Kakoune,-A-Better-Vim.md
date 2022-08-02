--- 
published: true
---

Vim has been the darling child of the Linux community since its conception. Vim is, apart from Vi, probably the most used text editor on Linux. And that's for good reason. Vim is super fast, extremely efficient, and has very sensible, albeit, hard to adjust to keybindings. But even though Vim is without flaws, it isn't  without some room for improvement. In fact, there is another text editor, that takes the core fundamentals of Vim, and builds on them to make an even better, even more programmer friendly editor. And it is very possible that you've never heard of it before. Kakoune is a super fast, easy to adapt to, and very efficient text editor that allows you to do everything that you would need to do in Vim, faster and with less keystrokes. I installed and played around with this editor, and I am going to give the overall rundown of how to use it, some of it's features, and some things that make it so unique. 

# Clippy 

Clippy is the creation of Microsoft, and it seems like blasphemy to use it in a FOSS text editor. But, unlike Microsoft's Clippy, the Clippy in Kakoune is actually helpful, and doesn't get in your way. When you go to run a command in Kakoune, much like you would in Vim, Clippy shows up as a little bit of ACII art in the bottom right corner, and explains what that command will do. This is super helpful if you are a new user switching over from Vim, and need to know that everything means. Clippy even helps with your keybindings. For example, if you press 'G', Clippy will show you all of the keybindings associated with 'G', and will explain to you what they will do. 

# Modes

Kakoune is a lot like Vim, so it makes a lot of sense that Kakoune would share the traditional Vi input, normal, and command mode's. However one thing you may notice right away is the lack of visual mode. Kakoune is designed in such a way that you'll be selecting text constantly, so there is no need for a visual mode. You can simply select a word, paragraph, line, or sentence, and either use 'y' to yank it, or you 'd' to delete your selection. 

# Keybindings

Although Kakoune is very similar, it is not Vim. Many of the keybindings aren't the same. So although most people will have a very easy time switching over, one will have to re-learn a few things. For example, many of the traditional Vim  keybindings are flip-flopped. This may confuse new users switching over from Vim at first, but eventually, it starts to make sense. In Kakoune, you can only do a command on something once you have selected it. You use "wd" instead of "dw", because you need to select the word before you delete it. And while there are some more minor differences, as long as you have a knowledge of Vim, and grasp that concept, you should be fine.  

# Look & Feel 

Any editor that has Clippy is bound to be stylish. And Kakoune delivers on all of the eye candy that you'll ever need. It comes pre-installed with a wide variety of popular themes (Nord, Gruvbox, etc.), and doesn't even require you to edit a config file to switch between them. And the autocomplete feature has a reasonable, easy to use, and easy to  understand popup allowing  you to autocomplete a word. The only part of this text editor that isn't absolutely gorgeous is the status bar, but I would by no means say that it looks bad. 

# Extensiblity 

In many cases, niche text editors are extensible, but don't actually have any plugins. And I am happy to say that for Kakoune, this isn't the case. There are tons of plugins available, including some of your favorites from Vim. Kakoune has their own version of NerdTree, Powerline, Plug, Todo, and every colorscheme under the sun. They even have their own [website](https://kakoune.org/plugins.html), where you can easilly download over 250 plugins. 

# Conclusion 

Kakoune is an editor, that until a day ago, I had never heard of before. But now that I have gotten a chance to use it, I am in love. I am not going to switch over, however I plan to use it on some Ubuntu servers where I can't install Emacs. It is lightweight, easy to use, and just so, soooooo smooth. If you are currently using Vim, and have an open mind, I would 100% recommend just giving Kakoune a try. You won't regret it. 
