---
published: false
---
Personally, I torrent a lot. I use torrents to download Linux ISO's, but also use them to download movies and TV shows. So, like every vital piece of software on my system, I'm very opinionated in terms of what I use. And after searching, finding, and using many different torrent clients, I have settled on Transmission. Transmission is a torrent client that can be used in many different platforms, under many different frameworks, including on the command line. So, if having a fully functional torrent client on the command line is something that appeals to you, I'll show you how you can install and use Transmission CLI on any Linux distro.  

# Installing Transmission

Depending on what Linux distro you use, feel free to copy-paste these command into your terminal to install the Transmission daemon and CLI program. 

## Ubuntu/Debian 

    sudo apt install transmission-daemon transmission-cli

## Fedora/CentOS/Rocky 

    sudo dnf install transmission-daemon transmission-cli 

## Arch/Manjaro/Endeavour
    
    sudo pacman -S libtransmission transmission-cli 

# Enabling the Transmission Daemon 

Before you can actually use Transmission, you are going to have to start the daemon. As long as you are using a distro with Systemd (You probably are) you can enable Transmission with this simple command. 

    sudo systemctl enable transmission-daemon

From there, you can either reboot into your machine, or start the daemon with this command. 

    sudo systemctl start transmission-daemon

# Using The CLI 

## Downloading 

Whether you have a torrent file or a magnet link, all you need to do is run *transmission-remote* with the *-a* flag followed by link or file in quotes, like so. 

    transmission-remote -a "TORRENT.torrent"

## Monitoring Your Download 

If you want to monitor your download, all you've got to do is run this command. 

    transmission-remote -l 

It should spit out an output that looks like this. 

	ID   Done      Have  ETA      Up    Down  Ratio  Status  Name
    1     0%       None  Unknown  0.0   0.0   None   Idle    TORRENT
    Sum:           None           0.0   0.0

## Removing a Torrent 

Now, ideally, you'd seed the torrent for as long as you possibly can, but eventually you've got to remove it. To do that, you're going to need to use the torrent's ID. This is the same ID that you can see when you run "transmission-remote -l". Then, once you know the ID, you can use this command. 

	transmission-remote -t ID -r

# Conclusion 

Whether you have a system with crappy specs, want to use MPV with framebuffer for a dedicated movie watching system, or just like using the terminal, transmission-cli is a easy, fast and effective way to torrent without ever having to touch a GUI.
