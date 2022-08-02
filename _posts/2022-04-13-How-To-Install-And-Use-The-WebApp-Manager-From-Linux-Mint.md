---
published: true
---
Why do you need to have so many apps installed? Seriously, in many cases, when you are running an app
such as Discord or Email, you could get just as much utility by running these things in a web browser. So, if you would like to skip actually installing an app, while still having all of the desktop functionallity of an actual natively installed apps, you can look to Linux Mint. Webapp-Manager will create desktop-integrated, fast, and isolated web apps for Linux. I am going to explain how you can install and use Linux Mint's Webapp-Manager on any Linux distro.

## Ubuntu

For installing on Ubuntu and Ubuntu based systems, for easy updating, you should add the PPA. You can do so with this command.

        sudo add-apt-repository ppa:kelebek333/mint-tools

Then, you can install with this command.

        sudo apt install webapp-manager

## Arch Linux

Installing on Arch Linux is quite easy if you are up to using the AUR. You can simply use your AUR helper, in my example, Yay.

        yay -S webapp-manager

## Other Linux Distros

Sorry to say, for other Linux distros, you will have to compile from source. If you don't know how to compile from source, you can simply run these commands.

        git clone https://github.com/linuxmint/webapp-manager

        cd webapp-manager

        sudo make clean install

After some waiting, it will be installed on your system.

## Usage

Webapp-Manager is very straitforward. Simply click the plus button to create a webapp. Then, you can add the name of the website, and the URL of the website. You can choose a 'Category', which will change what menu the app goes in. Then, you can choose which browser you would like to launch the web app in. From that point, you can simply open your menu and run it like any other app. If you would like to use extensions (Ublock Origin), you can simply type 'ctrl+t' to create a new tab, and then go and install the extensions how you would on a normal browser.

# Conclusion

In many cases, it is stupid to install an actual app, but we all still crave the convenience of a traditional desktop app. By getting the best of both worlds, and using these web apps, you can ensure that all of your favorite websites are at your fingertips, without ever having to open a conventional web browser. It also means that, without sacrificing convenience, you can run these apps without ever having to actually maintain or set them up on your system.
