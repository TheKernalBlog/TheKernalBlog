---
published: true
---
Gedit, the GTK text editor that was first released 23 years ago, has been replaced in the newest version of GNOME; dropped for the new Libadwiata 'Gnome Text Editor'. And, while Gedit is often made the butt of the joke by Vim and Emacs users, it is more alike then you'd think. Gedit is an amazing, extensible text editor that is packed full of features. So, I've been giving it a try. And I'm going to explain what makes Gedit so good, with the hope that maybe you'll take it more seriously. 

# Extensive plugins 

Gedit has more plugins than an extension cord for a high-end self hosted server room. Anything that you would like to accomplish on Kate, Emacs, or Vim can be easily achieved on Gedit. Do you want Vim input mode? A terminal emulator? LATEX and Markdown support? There's plugins for every last one of these, and much, much more. In fact, many of the most useful plugins can be installed on most distributions with the gedit-plugins package like so. 

## Ubuntu / Debian 

	sudo apt install gedit-plugins 
	
## Fedora/CentOS/Rocky 

	sudo dnf install gedit-plugins 
	
## Arch 

	sudo pacman -S gedit-plugins 
	
# Resource Usage 

Compared to other GUI text editors, Gedit is very lightweight. Although, terminal text editors such as Micro or Vim require many less resources, Gedit is on par with Emacs, and even better than Kate. I tested all of these text editors, with the markdown form of my previous blog loaded. Here are the results. 

## Gedit

- 81 MB of RAM

- 0% CPU usage 

## Emacs

- 74 MB of RAM

- 0% CPU usage 

## Kate

- 94 MB of RAM

- 1% CPU usage

# Keyboard Shortcuts 

Many Vim users brag about how effective they are editing without having to touch the mouse. Yet, Gedit has almost as many keyboard shortcuts as Vim. Vi totals at 63 shortcuts, and more can be added depending on what spin of Vi or Vim you are using. Yet, Gedit, which is often toted as being for beginners, has a total of 59 keyboard shortcuts. And these shortcuts are much more obvious and easier to remember than the Vim shortcuts. Gedit is much more keyboard centric than people give it credit for. 

# Conclusion 

Gedit isn't just the extremely crappy text editor for GNOME, it's an independent, GTK based, fast, extensible, and feature full text editor. Many people try many dozens of text editors that don't integrate with their desktop, or are super hard to learn and patch, when really, Gedit is the best choice for them. So, if you're a dev, maybe give your super bloated IDE or minimal Vim setup a rest, and give good ol' Gedit a try.
