---
published: true
---

If you have experience with CentOS, Fedora, and Redhat, there is a good chance that you have used or at least heard of SELinux. SELinux stands for, “Security-Enhanced Linux”. It isolates applications, so that your system is more secure. If you have already spent the time learning SELinux, it is good to use it on other Linux distro’s, so I am going to show you how to remove Apparmor if you are using Ubuntu, then install and enable SELinux on Ubuntu and Debian based distro’s. 

# Disabling AppArmor  
## Ubuntu Specific 

Ubuntu comes with AppArmor, which is very similar to SELinux, and because of this it is not advised to be using both of them at once. You can simply disable the systemd service like so. 

	sudo systemctl disable apparmor 

Then, if you would like to, you can remove AppArmor using this command. 

	sudo apt remove apparmor 

Once you are done with all of these steps, please reboot to stop AppArmor.

# Installing SELinux 

You can install SELinux and everything you need to get it working with this one command in the terminal. 

	sudo apt install policycoreutils selinux-utils selinux-basics 

# Starting and enabling SELinux 

To activate SELinux, you can just use this one easy command. 

	sudo selinux-activate 

Just because it is active, doesn’t mean that it is doing much. If you would like to gain the security features of SELinux, you need to use this command to set the SELinux ‘mode’ to enforcing. 

	sudo selinux-config-enforcing 

Then, to have SELinux start, you can just reboot your system. 

# Conclusion 

SELinux is an amazing tool from RedHat, as it allows you greater security and control over your system. So even on Debian and Ubuntu based systems, it is almost always worth it to install and enable it. Whether you are a Sysadmin, or just someone random who would like to secure their computer, I would recommend using SELinux on your system.
