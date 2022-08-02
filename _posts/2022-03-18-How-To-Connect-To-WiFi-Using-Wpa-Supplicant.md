---
published: true
---
If you are using a minimal Linux distro, connecting to the internet can be a little bit of a hassle. Yet, if you are installing a distro that does not come with a GUI, you will have to learn how to connect to the internet from the command line. So, if you would like to have WiFi without using a fancy GUI, I am going to show you how to use wpa_supplicant to find, connect, and setup WiFi network. 

# Finding Your Network Interface 

If you are going to connect to Wifi, you will need the correct network interface to put in your wpa_supplicant.conf file. Simply run this command and you will get it. 

        sudo ip link

This will display your network interfaces, in my case, wlp0s20f3. Make sure that you write this down, because it will be very important later. 

# Finding The ESSID Of The Network You Want To Connect To 

In most cases, you will already know your ESSID, or as it is commonly called, your network name. But, if you don't, you can list all of the available ESSID's using this command. 

        sudo iwlist NETWORKINTERFACE scan | grep ESSID 

# Generating The Config File  

Now, with the network password, you can set up your config file with this command. 

        wpa_passphrase ESSID PASSWORD | sudo tee /etc/wpa_supplicant.conf 

# Connecting Using Your Config File 

Now, you will have to simply start wpa_supplicant with the path to your newly created config file, and your network interface. Just use this command, and you will be all connected. 

        sudo wpa_supplicant -c /etc/wpa_supplicant.conf -i NETWORKINTERFACE

# Adding An IP Address 

While you are connected, you will realize that you do not have an IP address. No worries, you can add one with this command. 

        sudo dhclient NETWORKINTERFACE

# You're Done!!!! 

That's it! You are now connected to your WiFi network. You can use it like normal. Whether you are connecting as a start to get a full GUI set up, are using it for a headless server, or even just prefer to connect without a GUI or a TUI, using wpa_supplicant is a great way get internet access easilly from the command line.
