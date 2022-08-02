---
published: true
---
Flatpak is a great tool. It allows you to get almost everything that you could ever want, completely separated from everything else in your system. The main problem with being containerized is that the apps don't follow your system's GTK theme. Assuming that you have your GTK theme in the ~/.themes directory, I am going to show you how you can use Flatseal to apply the correct GTK theme. 

# Installing Flatseal

Assuming that you have Flatpak installed, and are using Flathub as your Flatpak repo,  just use Flatpak to install Flatseal with this simple command. 

	flatpak install com.github.tchx84.Flatseal

# Allow access to the ~/.themes directory. 

Once you startup Flatseal, you are going to have to click on the application that you would like to change the GTK theme for. Sadly, there is no way to do all of the apps at once using this method. Then, you are going to have to scroll down to 'Filesystem', where you will see the 'other files' option. Click on the add directory button and write '~/.themes' in the new line that pops up. 

# Changing the GTK Variable 

If you are to scroll down  a little bit, you should be able to find a heading that says, 'environment'. Under that you will possibly see some variables that are already there. Click on the plus sign, and another box should popup for you to type in. Just put this line according to the GTK theme you are using. 

	GTK_THEME=ThemeHere

In my case, it would look like this. 

	GTK_THEME=Nordic-bluish-accent-v40 

Once you do this, you should be able to close Flatseal and open up the app you just changed. You should see that it uses the new GTK theme that you just set. 

# Conclusion 

Now you are able to use Flatpak apps seamlessly without it looking super out of place. Whether you are just using Flatpak so supplement something that is not in your distro's repositories, or you are using an immutable OS like Silverblue, changing the GTK themes of Flatpak apps is a must. So go on, theme your Flatpaks to your heart's content, there is nothing stopping you now!
