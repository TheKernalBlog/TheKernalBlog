---
published: true
---
If you have created a new account, or just logged into your Linux Distribution you may not be able to use the sudo command. This is because the account is not in the sudoers file. I am going to go over how you can add a user to the sudoers file, either by using the usermod command, or by manually editing the sudoers file. 

# “Usermod” Method 

The first thing that you are going to do is log into your root account. This can be achieved by using this command. 

	su – root 

You will then be asked to enter your root password. This will log you into root so that you can run the usermod command with root privileges. Now, all that you need to do is to use the usermod command. Simply type this in your terminal. 

	sudo usermod -a -G sudo (Username) 

Now you will have root privileges for the user. However, some people may decide that  they want to do it manually, by editing the sudoers file themselves. This way is more reliable, but slightly harder. I will show you how to do it. 

# Manual Method

The first thing that you are going to have to do is to get root privileges. Type this in your terminal. 

	su – root

 Type your root password when prompted to log in as root. Now, type this command to edit the sudoers file. 

	sudo visudo 

This will open the sudoers file in whatever text editor is your default. Search for the part of the file that says, “User Privilege Specification”. You will see your root account in there. To add your user to the root file, simply type this in the “User Privilege Specification” section. 

	(Your Username) All=(ALL:ALL) ALL

Once you save the file, you should now be able to use root privileges with the user that you have added to the Sudoers file. 

 
You have now learned how you can add a user to the sudoers file. This can help when creating a new user for your computer, or when the install goes wrong and denies you root privileges. You should be able to use either of the methods to fix it.
