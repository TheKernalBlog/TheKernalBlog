---
published: true
---
With thousands of people switching to Linux every day, people are going to want to use Window managers. Window managers, as opposed to desktop environments, are bare bones. Some will have a panel, but they are mainly just managers for your windows. One of the most popular Winndow managers is i3. I am going to try and explain how to make use of the i3 config file, to customize, and become a true power user.

To edit the config file, you are going to have to find it. To find the config file, you are going to have to go into your file manager. Once there, you are going to need to show hidden files. In the home directory, you should see a file called .config. This has all of your config files in it. Open the “i3” file, and you should find the config file. Simply click on it to open in your preferred text editor.

Something that you should note is that whenever you write a command you have to give it a “name”. Basically you need to put a pound sign, followed by what you want to call the command. If I was trying to add a command to lock i3, it would look something like this.

"# i3_lock"

“Put_Command_Here”

You need to do this before you add anything to the config file. Keybinds, applications to autostart, and anything else.

One of the many reasons that you would use i3 is that you like using your keyboard. So, it goes to show that most i3 users would like to add their own keybinds. How can this be done? It is very simple. You use the bindsym commend in the i3 file. You are going to need to type bindsym, the keys that you want to press, and then exec followed by what you want to run. For example, if you want to make a keybind to run i3lock, you would type.

bindsym $mod+x exec i3lock

Keep in mind that “$mod” is the super/windows key. You can do this for your browser, file manager, text editor, or anything else you may want.

There are many programs that we would want to autostart whenever we log in. Like your panel or background manger. This can be achieved easily in i3. All that you need to do is type this command.

exec — no-startup-id “APPLICATION” –restore

This will restore the application whenever you log in to i3. This is crucial if you want a different panel or wallpaper.

With these tips in mind, I hope that you can make yourself more productive and/or make your desktop look cooler. Using i3, there are no limits, and this is just scratching the surface. You can always learn more about this amazing window manager. The sky is the limit!
