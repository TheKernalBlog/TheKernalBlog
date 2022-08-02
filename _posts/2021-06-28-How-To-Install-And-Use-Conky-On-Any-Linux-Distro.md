---
published: true
---
We all want to make our Linux desktops look better. You can install docks, change icons, switch window managers, but there is something else that it gaining more steam. Conky. Conky allows you to display system information on your desktop, making it look better. This information can be ram, cpu, or gpu usage. Even time or date. I am going to try to walk you through the steps of installing and using Conky.

To use Conky you are going to have to install it. Conky is in most package managers. It is available on RedHat, Arch, And Debain based distros. Here are the commands to install.

Debain/Ubuntu: sudo apt-get install conky

Redhat/Fedora: sudo dnf -y install conky

Arch: sudo pacman -s conky

You will realize that when you run it by typing “conky” in the terminal, it does not look good. So, you need to install some themes. Conky themes change the look of your Conky and make them look better. You can usually just look up “conky themes” to find them, but I think that (1) shows some of the best themes.

Now that you’ve got your Conky theme downloaded, how to you add it to your desktop. Most Conky themes are zipped. You should extract/unzip them. In that file, there should be a text file. Take that text file, and rename it “.conkyrc”. Then move it to your home directory. Simple as that. Now when you start Conky by typing “conky” in the terminal, you should see your Conky theme on the desktop.

Now all that you need to do is autostart it. Most DE’s have a application to autostart a program. Simply search “autostart:” in your desktop environment and add “conky”. If you want to see how to do this on i3, look at my previous guide.

If you have followed my instructions every time you boot in you should have the beautiful Conky widget of your choice. There are hundreds of Conky themes out there, so feel free to experiment. Eventually, you will find the perfect Conky for you.

1: https://www.ubuntupit.com/best-conky-themes-for-linux/
