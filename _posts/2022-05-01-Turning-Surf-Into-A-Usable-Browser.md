---
published: true
---
Other than init systems and distros, there is nothing that Linux users like arguing about more than browsers. "Ungoogled Chromium is the best", "No LibreWolf is the best". Well, there is one browser that is made specifically for Linux and BSD, that many people ignore. But it turns out, that with a little configuration, it can be not only a very fast, but feature rich browser. So, I will explain how you can take Suckless's Surf browser, and make it a browser that it on par with other browsers, with tabs, a search engine, XDG compliance, and even smooth scrolling.

# Installing Surf & Tabbed

Surf is a tricky beast. If you don't have the latest version of WebKit or GTK installed, you should expect hell if you are planning to build from source. So, if you are on a stable Linux distro and don't want to build your own version of WebKit, you can install Surf with one of these commands.

## Surf

### Debian/Ubuntu

	sudo apt install surf

### Fedora

	sudo dnf install surf

### Arch Linux

	AURHELPER -S surf-git

Or, if you have the newest versions, or built them from source, and want smooth scrolling, XDG compliance, and a search engine, build like so.

	git clone https://git.suckless.org/surf

	cd surf

	make clean install

## Tabbed

With Tabbed, there aren't any dependency issues, so it is advised that you install it the same way you would most Suckless software.

	git clone https://git.suckless.org/tabbed

	cd tabbed

	make clean install

## Using Tabbed with Surf

If you are using a traditional app launcher like dmenu or Rofi, you can simply type "tabbed surf -e". But, if you don't want to do that every time, you can simply create a keybinding, shortcut in your desktop environment, or even an alias in your .bashrc or .zshrc.

## Adding a search engine, XDG compliance, and smooth scrolling.

### Downloading the .diff files

Before you can patch Surf for the desired changes, you need do download the .diff files. Using curl, you can download these patches like so.

	cd surf

### Web search

	curl -O https://surf.suckless.org/patches/web-search/surf-websearch-20190510-d068a38.diff

### XDG compliance

	curl -O https://surf.suckless.org/patches/xdg/surf-xdg-2.0.diff

### Smooth scrolling

	https://surf.suckless.org/patches/smoothscrolling-via-GTK3/surf-0.7-smoothscrolling.diff

## Patching

Patching suckless software isn't hard at all. Just type,

	patch -i FILENAME

and then recompile with.

	make clean install

# You're Done!

You can now use the Surf browser with tabbs, a search engine, XDG complicance, smooth scrolling, and whatever else you would like to add. It allows you to have a usable browser that works on even the oldest of computers. Plus, you can rub your amazing choice of browser in the face of people arguing about Chromium/Firefox.
