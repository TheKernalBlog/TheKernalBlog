---
published: true
---


Touchscreen monitors. Some people love them, and some people hate them. In my opinion, they are not very good. With registering inputs when there is no touching, to registering inputs anytime that you move them. So, some people will want to disable it. Luckily, this can be done fairly easily. 

To disable the module, you are going to need to find the name of the module. This can be achieved by putting this command in the terminal. 

lsmod | grep touch. 

This will give you the name of the module. In my case, the name of the module is “hid_multitouch”. Yours might be the same, but it most likely will be different. Make sure that you don’t forget this. 

You will need to use a text editor of choice. I like gedit so that is what I will use. You need to open your text editor in root so that you can add it to your  /etc directory. To open it in root type this in the terminal. 

sudo “name of text editor” 

You are going to have to add two lines. For the first one, you need to give it a “name”. Just type a # and then whatever you want to call it. I named it this. 

"# Disabling the module"

The second line is the most important. This is where you blacklist the module. Simply type this on the second line. 

blacklist “name of module” 

You are almost done. You are going to have to save the file. Make sure that you save it in /etc/modprobe.d. Name it whatever you want, but make sure that the file ends in .conf. Finally, you can save it. 

Congrats! Now as soon as your reboot you should notice that the touchscreen no longer works. I hope that if you are having problems with your touchscreen, this has helped you.
