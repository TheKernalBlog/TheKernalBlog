---
published: true
---
I2P is an anonymous, decentralized, peer to peer network, that aims to create it's own internet. It allows for un-censored, secure, and hidden communication. Many people under scrutiny from the government flock to I2P, as it is currently the best way to be anonymous. But, it can be a pain to install. So, I'll explain how you you can install, run, and configure I2P, so that you can have access to the safest , least exploited parts of the internet. 

## Installing I2P 

Before you can correctly install I2P, you need to install Java. If it is not already installed, you can use one of these commands. 

### Debian/Ubuntu 

	sudo apt install default-jre

### Fedora/CentOs/RHEL

	sudo dnf install java-latest-openjdk

### Arch/Artix/Manjaro 

	sudo pacman -S jdk-openjdk

Then, you need to download the I2P Jar file. Just go to [THIS](https://geti2p.net/en/download) link, and scroll down to 'Download I2P for Linux / BSD / Solaris'. Then, click the link to download the .jar file. Once you have it downloaded, use this command to install it. 

	java -jar i2pinstall_VERSION.jar

or, if you would like to do it without a GUI, you can use this command to install it without it bringing up a pop up menu. 

	java -jar i2pinstall_1.7.0.jar -console 

## Running I2P 

To start I2P itself, all you have to do is run 

	i2prouter start 

, and you can stop it like so

	i2prouter stop 

. But, you still have to configure your browser. Unless you are using a completely serperate browser, I would recommend creating a new browser profile, just for I2P Then, you need find your proxy settings. You should use a HTTP and SSL proxy, pointing toword localhost (127.0.0.1), with the port '4444' 

It is also worth noting that if you use Firefox, you should open 'about:config', and ensure that the setting 'media.peerConnection.ice.proxy_only' is true. 

## Configuring I2P 

Once your browser is all set up, you can get to configuring I2P itself. To start off, you must open your browser and put '127.0.0.1:7657' in the address bar, which will bring you to a configuration page. From there, you need to decide how much you would like to put into the network, and how much you would like to have for yourself. If you don't want to make the decision, there is a test that will determine it for you. Once you are done, you can start browsing. 

# You did it! 

Now, all there is to do is find some Eepsites and start browsing. You can organize, talk, and even email without any fear of being tracked by Google or the Feds. And, if you are that kind of person, I2P is a pirate's dream.
