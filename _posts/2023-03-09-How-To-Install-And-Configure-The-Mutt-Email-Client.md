---
published: true
--- 

Email is one of the most useful pieces of technology to have been created in the past 50 years. Sure, it may not be as flashy as high speed video streaming or as complicated as neural networks, but it's revolutionized the ways that a most people work and communicate. The ability to instantly send a message to anyone in the world with virtually no cost is revolutionary. And part of Email's appeal comes with the wide variety of options for how you want to interface with it. One of the most important choices you make when using Email is what client you want to use. And today I'd like to highlight one Email client in particular: Mutt. Mutt is a terminal based Email client that doesn't mess around. Almost anything you'd want to do in Thunderbird or Outlook can be done on Mutt, with less bloatware and more efficiency. So if that sounds good to you, here's how you can install and configure the Mutt Email client. 

# Can You Use Mutt? 

Sadly, depending on what Email you use, Mutt just won't be an option. Mutt requires IMAP ind SMTP servers from your Email provider, and this age, that's becoming less and less common. If you're using one of the more mainstream Email providers like Gmail, Outlook, Hotmail, or Yahoo, you should be fine. But Protonmail, Tutanota, and other privacy centric free email providers usually restrict IMAP and SMTP for paid users. However, there are exceptions. [Disroot](https://disroot.org) is a free, anonymous, and open sourced Email provider that provides IMAP and SMTP with zero cost. And so far, I've had a very good experience with them. 

# Installing Mutt 

Mutt has almost no dependencies and is very simple to install. Feel free to copy-paste one of these commands into your terminal depending on what distro you use. 

## Ubuntu / Debian 

    sudo apt install mutt 

## Fedora/Rocky/CentOS

    sudo dnf install mutt

## Arch/Artix/Manjaro

    sudo pacman -S mutt 

# Connecting your IMTP & SMTP servers to Mutt. 

Almost every Email provider has a page with their posted IMAP and SMTP addresses and ports. Before you do anything, search those up. 

To configure Mutt, you're going to need a muttrc file. You can create it like so. 

    mkdir ~/.config/mutt/

    touch ~/.config/mutt/muttrc

Then, to connect to IMAP and SMTP, add these two lines to your config file, replacing the bold elements with the addresses and ports of your preferred Email provider. 

    set folder = "imaps://Name@Email.com@Server.com:Port"
    
    set spoolfile = "+INBOX" 

    set smtp_url = "smtp://NAME@EMAIL.COM@SERVER.COM:PORT"

Now, when you launch Mutt, you should be able to check and respond to Emails. But, you'll have to enter a password when you log in, and when you send an Email. This can get a little annoying, so, if you wish to, you can counteract this by adding these two lines to your *muttrc*, replacing the bold text with your Email password. 

    set imap_pass = "PASSWORD" 

    set smtp_pass = "PASSWORD"

# Adding Your *from* and *realname* addresses. 

Now that you can actually use Mutt, you're going to want a from and realname address to ensure that everything goes smoothly. Add these two lines, inserting your Email address and real/fake name respectively. 

    set from = "NAME@EMAIL.COM" 

    set realname = "NAME NAME" 

# Creating different Mailboxes 

If you use a graphical Email client, you're probably used to different Email boxes, where, for example, you can view your drafted or sent Emails. And as it turns out, that's entirely possible on Mutt. Just copy these few lines into your *muttrc*. 

    set record = "+Sent" 
    set trash = "+Trash" 
    set postponed = "+Drafts" 
    mailboxes =INBOX =Sent =Trash =Drafts =Junk 

# Setting Your Editor 

Finally, you get to choose which text editor you wish to use for writing Emails. Set it by copying this command into your *muttrc*. 

    set editor = "*EDITOR*" 

# You did it! 

Now, if you've followed my guide correctly, you should have Mutt in a working state, with an effecient, streamlined Email experiance featuring multiple Mailboxes. You can answer your Email the way that it was meant to be answered, not in a bloated web interface or overly complicated modern Email client. And once the muscle memory clicks in, you'll be more efficient and productive than ever. Because while Mutt, just like Email, may not be flashy or impressive, it's one hell of an amazing tool. 
