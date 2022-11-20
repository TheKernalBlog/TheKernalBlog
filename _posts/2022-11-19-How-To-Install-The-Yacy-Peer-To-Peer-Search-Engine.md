Chances are, if you're as paranoid as me, you've used a wide variety of search engines. Every couple months or so, I'd find a shiny new search engine that claims to be faster, easier, or, most importantly, better for privacy. I've used DuckDuckGo, Searx, Metager, Startpage, Whoogle, and more. But recently, while trying to set a VPN on my homelab, a new search engine caught my eye. I had discovered Yacy: a different kind of search engine. Yacy is a self-hosted, peer-to-peer search engine that completely throws all conventions out the window. And so, if you'd like to give it a whirl, I'll show you how you can install, configure, and use Yacy as your search engine.


<a id="org80eb436"></a>

# Installing The Dependencies

Yacy itself only has one dependency, Java 8. However, to install it, you're going to need tar and wget. Chances are, you already have tar and wget installed, but I'm going to show you how to install them anyway.


<a id="org16313bf"></a>

### Ubuntu/Debian

`sudo apt install openjdk-8-jre-headless wget tar`


<a id="orga100a04"></a>

### Fedora

`sudo dnf install java-1.8.0-openjdk wget tar`


<a id="org79b6aa2"></a>

### Arch Linux

`sudo pacman -S java8-openjdk wget tar`


<a id="org0ff29d0"></a>

# Downloading, Unpacking, and Running Yacy

Now, you have to use wget to download a compressed file from the official Yacy website, and then use tar to extract it, like so. 

`wget https://download.yacy.net/yacy_v1.924_20210209_10069.tar.gz`

`tar xfz yacy_v1.924_20210209_10069.tar.gz`

And to finally start Yacy, you just cd into the extracted directory and run the shell script.

`cd yacy`

`./startYACY.sh`


<a id="orga8212ba"></a>

# Starting Yacy on login

Chances are you'd rather not manually cd into the directory and start Yacy manually every time you restart or log in. Thankfully, there's a few ways you can go. But what I'd recommend is starting it with your .profile.

Just open it up

`TEXTEDITOR ~/.bash_profile`

and then add the path to the start Yacy script.

`/path/to/yacy/startyacy.sh`


<a id="orgc6e2d2b"></a>

# Using Yacy on Firefox

![YacyImage](/images/Yacy.png)

Now you've got Yacy, and you can access it at any time by going to to localhost:8090. But there's no way to make it your default search engine by normal means. You need the open sourced [Search Engine Helper](https://addons.mozilla.org/lv/firefox/addon/search-engines-helper/) from the Firefox addons store. Open the extension, click 'Add a New Search Engine'. Then, add this URL `localhost:8090/yacysearch.html?query=%s`, and whatever image and name you want. Once you do that, you should be able to select your new search engine in *about:preferences* like you would any other.


<a id="org204e4a8"></a>

# You're Done!

That's all there is to it! You've got a completely usable, private, open sourced, peer-to-peer search engine running locally on your computer. It may be a little slow, and it may eat up a few resources on your computer, but I'd say that for what you're getting, that's a more than fair trade. If you're paranoid and crazy, you'd be crazy not to use it. 


# Table of Contents

1.  [Installing The Dependencies](#org80eb436)
        1.  [Ubuntu/Debian](#org16313bf)
        2.  [Fedora](#orga100a04)
        3.  [Arch Linux](#org79b6aa2)
2.  [Downloading, Unpacking, and Running Yacy](#org0ff29d0)
3.  [Starting Yacy on login](#orga8212ba)
4.  [Using Yacy on Firefox](#orgc6e2d2b)
5.  [You're Done!](#org204e4a8)
