---
published: true
---

For so long, Suse Linux has a monopoly on a graphical managment service for Linux. While YaST is a great tool that I absolutely adore, it sucks that you can only run it on SUSE and SUSE based Linux distros. However, it seems that there is a saviour. Our friends at Red Hat have created Cockpit, a web based, extensible, and powerful GUI that allows you to configure and automate many jobs on Linux that would otherwise require using the command line. So, If you would like to manage your servers without having to type out a bunch of commands, I am going to explain how to install, configure, and run Cockpit.

## Installing Cockpit

If you are going to install Cockpit on Debian or  Ubuntu, either copy-paste or type out this command.

        sudo apt install cockpit

Or, if you are following this guide on Arch, you can do the same with this command.

        sudo pacman -S cockpit

## Running The Cockpit Service

Using Systemd, you can enable the Cockpit socket to run as a daemon whenever your boot into your Linux distro with this command.

        sudo systemctl enable cockpit.socket

Plus, if you would like to start the Cockpit socket right away without rebooting, you can use this command.

        sudo systemctl start cockpit.socket

## Opening The TCP port

Cockpit uses the TCP port 9090 to allow it to run in your browser. So, in order to get Cockpit working, you have to unblock the port on your Linux firewall. The simplest way to do this is by using 'ufw', which is pre-installed on Ubuntu, but not Debian or Arch. So, if you don't already have it, you can install it like so.

### Debian

        sudo apt install ufw

### Arch

        sudo pacman -S ufw

Then, you can actually open the port with this command.

        sudo ufw allow 9090

## Opening Cockpit In Your Web Browser

Assuming that you already have a graphical web browser installed, you just have to put this in your URL bar, making sure to use your actual system hostname.

        http://HOSTNAME:9090

From there, you will have to enter your username and password.

# You're Done!

You have now instaled and opened Cockpit in your web browser. You can finally scoff at those fancy SUSE users as you manage services, logs, storage, and even virtual machines all from your browser. Now, you can control your entire system, without having to so much as type a word. Plus, if you have a bad memory like me, it is a lot easier than remembering every single command in existince.
