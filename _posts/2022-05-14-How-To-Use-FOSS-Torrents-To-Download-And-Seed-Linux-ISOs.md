---
published: true
---
If you are testing Linux distros, or just like distro hopping, the chances are that you're downloading a lot of ISO files. But, that can be quite a hassle, especially if you are downloading large amounts. It would be nice to have all of your ISO's in one place, Right? Well, thanks to FOSS Torrents, that is possible. I'll show you how you can download torrenting software, find ISO's, and even help out less fortunate Linux distros by seeding their ISO's. 

## Downloading Your Torrent Client 

There is a lot of software available for torrenting, and I'm not not going to say that one is better than the other. However, I personally would reccomend Transmission or QBitTorrent to beginners. So, depending on which you would like to install, and your Linux distro, you can use one of these commands. 

### Ubuntu/Debian

	sudo apt install transmission

	sudo apt install qbittorrent

### Fedora/CentOS/Rocky

	sudo dnf install transmission

	sudo dnf install qbittorrent

### Arch Linux 

	sudo pacman -S transmission

	sudo pacman -S qbittorrent

## Grabbing Your Torrent File

In order to Torrent a file, you need to grab the .torrent file from [Right Here](https://fosstorrents.com/distributions/). You'll see a screen that [looks like this](https://github.com/TheKernalBlog/TheKernalBlog.github.io/blob/master/images/Screenshot%20from%202022-05-14%2014-13-38.png). Then, it's as simple as searching for the distribution that you want to download, clicking on it, and clicking download the torrent file you would like to use. From there, if it doesn't automatically open the file in your torrenting application, you can press CTRL + O in your preferred app, and open the .torrent file that way. 

## Seeding ISO's 

One of the easiest things that you can do to help Linux distros without having to contribute money is seeding their torrents. And FOSS Torrents provides the perfect way to do that. It's as simple as downloading a boat load of .torrent files for various different Linux distros, and then opening them all in your preferred torrenting application. From there, you can wait for them all to download, and leave your torrenting app open. This will seed the torrent, which will make the torrent faster for then next person who will download it. Then, when you feel that you have dome enough, you can simply stop the torrent program and delete all of the files. 

# Conclusion 

FOSS Torrent is an amazing tool that deserves more recognition. It is the one place with almost every Linux distro and BSD derivative you could ever need. It allows for smaller Linux distos to deliver their ISO's without having to pay the expensive costs for hosting their own servers. Plus, there really is nothing better feeling than downloading 10+ ISO's at the same time, and then seeding them afterwords.
