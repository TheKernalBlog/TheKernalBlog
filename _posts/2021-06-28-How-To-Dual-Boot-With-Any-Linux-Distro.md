---
published: true
---
When it comes to installing a linux distro, some people need to dual boot. Whether it is with Windows for propietary software, or with another linux distro in case it fails. However, most installers for linux distros will not have a flat “dual boot” option in their install. They almost have a manual partitioning tool. I am going to try to explain how partition your disk so that you can dual boot linux with your other operating system of choice.

The first thing that you are going to need to do is create space. This Is pretty simple. You can shrink the space in the operating system that you already have. Or, I just prefer to use a live usb and shrink it with Gparted. Once it is shrunk, you can boot in the usb that you are going to install with and go to the manual partitioning tool.

The second thing that you are going to want to make is a swap file. This can also be called a “page” file. This is a place where your computer can store information when you are using all of your ram. This allows your computer to not only run faster, but open more apps. The steps to do this are pretty simple. You need to create a partition the size of half your ram. For example, I have 8gb of ram, so I would make a 4gb swap file. When asked what to use it as, use it it as “linux swap” or simply “swap”.

The third thing that you need to do is to make a efi partition. This is what you are going to boot into. The size can be from 150–500mb. I would use 500 just to be safe. Compared to the size of your hard drive 500mb isn’t to much space. Make sure that this is called “efi”, and is put into /boot/efi. If you have the choice to choose where the boot file goes make sure that it is in this partition.

The last thing that you are going to have to do is make a root partition. This is where all of your files will be. Make sure that this takes up all of the rest of the space. You should call it “/” and make sure that it is ext4. This is the most simple one to make.

If you have followed all of these directions, you should be able to install and dual boot. This applies to every linux distro with a gui installer. While some linux distros have the choice to automatically dual boot, making sure that you manually partition is the safest, and most reliable way to dual boot.
