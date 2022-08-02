---
published: true
---
If you are a tech savvy Linux user, chances are you are self hosting a couple services on either your main machine, a Raspberry Pi, an older Laptop/PC, or even a VPS. I myself have a server seeding various Torrents, running a TOR relay, OpenVPN, and even Nextcloud. However, it can be a little annoying having to SSH into your server every day just to run a simple 'apt update && apt upgrade'. Sometimes, you just want to set it and forget it. But luckily, if you're like me and use Ubuntu for your servers, you can quite easily have automatic updates applied every day. So, I am going to show you how you can install and get automatic updates, with the ability to send notifications directly to your Email. 

# Installing 'unattended-upgrades'

Whether you are using Ubuntu server or Desktop, this should already be installed. But just in case, you can run this command to install it. 

	sudo apt install unattended-upgrades 
	
# Enabling Auto Updates Every Day 

You can manually edit the "*/etc/apt/apt.conf.d/20auto-upgrades*" file, and if you don't want to update every day, it's your only option. However, I personally would recommend this method, as it is much less complex. Simply copy this command into the terminal. 

	sudo dpkg-reconfigure -plow unattended-upgrades
	
It will show a screen that looks like this. 

![TUI](/images/Unattended-Upgrades.png) 

Just select yes, and it will immediately edit the file for you, setting all of the values to "1", causing your system to update every day. 

However, if you would like to, you can create/edit the file yourself, replacing the "1's" with however many days you would like to go between updating. Here is an example, if you don't already have the file. 

![FILE](/images/Unattended-Upgrades-File.png) 

# Setting Up Email Notifications 

As the updates are automatic, there is always some risk, as there would be if you were installing the updates manually. But if something goes wrong, you would like to be notified, right? Thankfully, you can send yourself an Email using Mailx without too much hassle. To start off, install Mailx. On Ubuntu, you can install the BSD version with this command. 

	sudo apt install bsd-mailx
	
 Now, open "*/etc/apt/apd.conf.d/50unattended-upgrades*" and get ready to edit. You should see a line that looks like this. 
 
	//Unattended-Upgrade::Mail "";
	
Uncomment it, and put your Email address in those quotes. The line should look like this, but obviously with the Email address switched out for an actual Email. 

![EMAIL](/images/Unattended-Upgrades-Email.png) 

# You did it!! 

Now, every day, or however long you set between updates, your server will update all on its own, and send you a handy Email to go along with it. This is super helpful if you have a large amount of severs, or like me, are just lazy. If anything, it beats coming back from a long trip and having your server break after it amassed hundreds of outdated packages, which wold obviously ***never*** happen.
