---
published: true
---
When I write all of my distro reviews, I am obviously testing then in a virtual machine. When doing this testing, I always opt for Virt-Manager. Virt-Manager uses KVM, which is build directly into the Linux kernel, so it will bring an experience much closer to running on native hardware. If you would like to get away from oracle and have a faster and better experience for virtual machines, I am going to show you how to install virt manager along with QEMU and KVM.

# Installing Virt-Manager and dependencies 

Depending on what Linux distro you are using, copy-paste this command in your terminal.  
  
## Ubuntu/Debian               

        sudo apt install qemu libvirt virt-manager

## Fedora/RHEL/CentOS

        sudo dnf install qemu libvirt virt-manager

## Arch Linux 

        sudo pacman -S qemu libvirt virt-manager

# Enabling the Libvirt daemon 

In order for KVM and QEMU to work, you need to have the Libvirt daemon running in the background. You can do this with systemd like so. 

        systemctl enable libvirtd

This will enable the daemon every time that you boot. You can either reboot, or just type this command to that the daemon right now.

        systemctl start libvirtd 

# Adding your user to the Libvirtd group 

Despite everything being installed and running, you will realize that you still can't use virt-manager. This is because you are not added to the Libvirtd group. No worries though, you can add yourself to the Libvirtd group with the usermod command like so.

        usermod -G libvirtd -a USERNAME  

# Conclusion 

You can now use Virt-Manager. Everything is set up, and you can slap in a iso image and boot up a virtual machine. And, while KVM is usually used for big headless servers, Virt-Manager makes it one of the best ways to test out and use desktop Linux distros. If it is good enough for sysadmins, it is good enough for you. So go, say no to Oracle, and install Virt-Manager.
