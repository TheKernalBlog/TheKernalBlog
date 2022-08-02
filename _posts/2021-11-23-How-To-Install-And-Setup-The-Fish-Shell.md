---
published: true
---
A Shell is the program that allows the user to access all of the features of the operating system. The most commonly used shell is "Bash". Basically every single  Linux distro uses the bash shell. But that does not mean that there are not other shells. One shell that had been gaining popularity is the "Fish" shell. With it's customizability and autocompletion, many Linux and Mac users have made the switch to Fish. I am going to go over how you can install Fish, switch away from bash, and then how you can get it to a usable state. 

# Instillation 

Depending on what Linux distro you use, copy-paste these commands in your terminal.  

## Fedora

	sudo dnf install fish

## Debian/Ubuntu

	sudo apt install fish

## Arch

	sudo pacman -S fish

# Switching to Fish

Now that you have it installed, you can try it out by typing "fish" into your bash shell. However, if you would like to use it as your main shell, you can do so using the chsh command. Make sure that you don't run this with root permissions, as you may accidentally switch the root profile to fish instead of your own. 

	chsh -s /bin/fish USERNAME


# Setting up fish

## Fish_config

The easiest way that you can configure Fish is using the "fish_config" command. When you type this in your terminal, it will open up a HTML file in your browser, providing you a easy to use GUI for changing the colors, look, functions, variables, and much more. 

## Removing Welcome Prompt

Fish automatically starts with a promopt that says, "Welcome to Fish". This can become annoying. The easiest way to change it is to edit the config file for fish. Simply use your favorate text editor like so. 
	
    TEXTEDITOR ~/.config/fish/config.fish
 
All that you need to do is copy-paste this line into the file. 

	set fish_greeting 


Just use that line if you would like to get rid of the greeting altogether, but if you would like to add your own custom greeting you can just add your own text. 

# Conclusion

While bash may be more popular, fish is a great shell. It is super easy to learn, plus the autocompletion is just amazing. There is no reason not to try it out. It's super convenient, fast, and beautiful.
