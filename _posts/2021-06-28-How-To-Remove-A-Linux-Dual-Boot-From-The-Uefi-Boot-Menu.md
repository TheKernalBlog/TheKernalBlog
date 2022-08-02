---
published: true
---
For a lot of Linux users, you are doing a thing called distro hoping. This is where you install a bunch of Linux distributions to find the one that you really want to install. The only problem is, this leaves behind the empty shell of the linux distro in your boot menu. If you want to boot automatically into your operating system this can be a big problem. I am going to show how you can successful remove a boot option from the boot menu. 

The first thing that you are going to need to use in “efibootmgr”. This is already installed on a bunch of linux distributions. If not, you can install it with apt, DNF, or pacman. Once you are sure that you have it installed, type “efibootmgr” in the terminal. You should get a list of all of the OS’s in your efi boot folder. Each of them will have a number. Find the number of the operating system that you want to delete and type this. 

Sudo efibootmgr -b (Boot Number) -B

You may think that you are done, but you still need to actually remove it from the efi folder. To find the name of the operating system type this in the terminal. 

cd /boot/efi/EFI 

ls

You should now see a list of every efi file on your system. To remove it, simply put this command in the terminal. 

Sudo rm -R “Name Of Operating System”. 

Congrats! When you boot up again you should not see these boot options in the boot menu. Hopefully that has helped you, and have fun distro hopping!
