---
published: true
---
When Red Hat announced that CentOS would be the upstream from RHEL, many people were upset. The stability and enterprise grade software that is offered from CentOS is something that many people relied on for servers or desktop usage. However, Rocky Linux is now a amazing alternative to CentOS, doing exactly what CentOS used to do. Instead of re-imaging your systems, I am going to show you how you can migrate your CentOS system to Rocky Linux while still being able to save all of your files and configurations. 

Before you do anything else, make sure that your system is fully upgraded. You can do this by running this command. 

	sudo dnf -y update

Go ahead and reboot if you saw that your Kernel, or another part of the operating system was updated. I would reboot just to be safe, so that you can be sure that nothing will break. 

Rocky Linux has a very convenient script called migrate2rocky. You will need to download the script, and make sure that you have curl installed. Then run this in your terminal. 

	curl -O https://raw.githubusercontent.com/rocky-linux/rocky-tools/main/migrate2rocky/migrate2rocky.sh 

You have the script, but unless you make it executable nothing will happen if you run it. There are ways of doing this where you can use a GUI, but I prefer just using the chmod command in the terminal. 

	chmod +x migrate2rocky.sh

Now everything should be set up to actually run the script. Make sure that you run this with root permissions. Keep in mind, this will take a long time, as it has to change all of the CentOS repositories to Rocky Linux repositories. Run this in the terminal to start the migration. 

	sudo bash migrate2rocky.sh -r

You are almost done. You will have to sync your distro with Rocky Linux. To do this, run this in your terminal. 

	sudo dnf distro-sync -y


# You’re Done! 

Now as soon as your reboot, you should see the Rocky Linux Grub Bootloader. You will now be able to continue using the super stable, rock solid operating system that you are used to. Once again being the downstream of RHEl. 

If you would like to lern more about Rocky Linux, you can check out their site here. (Unclickable For Your Security) 

rockylinux.org
