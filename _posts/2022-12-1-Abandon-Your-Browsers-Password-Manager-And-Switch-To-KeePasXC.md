---
published: true
---

Every day, there are hundreds and thousands of Email addresses and passwords released in huge data breaches. No matter how unique or strong your password is, if you re-use it, and one of your accounts is compromised, all of your accounts are compromised. For that reason, password managers are becoming incredibly popular for both the paranoid privacy enthusiast and regular person. Sadly though, many of these password managers are closed source, built into the browser, or stored in the cloud. It's certainly better than nothing, but if you really want the best of the best without having to pay the money to host your own server, one option stands out from the rest. KeePassXC is a FOSS solution that provides you with all of the luxuries of a built-in browser password manager, with the security and peace of mind that comes with storing your passwords on a local encrypted file. If you're interested, I'll show you how you can install KeePassXC, create your database, and integrate KeePassXC flawlessly with your browser.


<a id="org3b52d73"></a>

# Installing KeePassXC

If you're to lazy or competent to install KeePassXC yourself, you can just copy paste one of these lines into your terminal depending on what distro you use.


<a id="orgf4a3eae"></a>

## Ubuntu/Debian

`sudo apt install keepassxc`


<a id="orgf68b2d4"></a>

## Fedora/CentOS/

`sudo dnf install keepassxc`


<a id="orgbc7b3e5"></a>

## Arch/Manjaro

`sudo pacman -S keepassxc` 


<a id="org50119a9"></a>

## OpenSUSE

`sudo zypper in keepassxc`


<a id="org4d0af46"></a>

# Creating a database

Now that you have KeePassXC installed, you need to create a database. Go to the very top left, and then click on "*New Database*". You'll be asked to give the database a name, and an optional description. Once you hit "*continue*" you'll be prompted to choose your encryption settings.


<a id="org4971603"></a>

## Encryption Settings

![img](/images/EncryptionSettings.png)

There is a slider ranging from 100 milliseconds to 5 seconds. The higher the decryption time, the more protected you'll be from brute-force attacks, but it can be very inconvenient. In most cases, the default encryption will serve you well.


<a id="org58ab6da"></a>

## Password Creation

![img](/images/PasswordCreation.png)

Here, you'll be asked for a password. Choose something that's easy to remember, but also incredibly difficult to guess. A song lyric, memorable sentence, or a tagline for a book are all great options. You may also want to create a key file. If you click on "add additional protection" you'll be greated with a prompt where you can create or source one of these key files. This will make your database much more secure, but it requires you to source the file every single time you want to unlock KeePassXC, and if you delete it, you're screwed.

Then, save the .kbdx file anywhere on the system and you're done! 


<a id="orgde89e99"></a>

# Creating an Entry

![img](/images/CreatingAnEntry.png)

Creating an entry is very simple. Open the database, and then select "*Entries*" in the top left corner, before selecting "*New Entry*". Then, you can enter or generated a password, put in a username, and add the URL. I always use KeePassXC to generate passwords, then change the passwords on existing accounts to the new, extremely secure password.


<a id="org2a795fd"></a>

# Using the Browser Extension

![img](/images/BrowserIntegration.png)

The browser extension makes using KeePassXC 100x easier. Instead of having to copy-paste the username and password into the field every single time you want to log in, you can just connect to KeePassXC using the browser extension and have it fill out the form for you. You can install the browser extension on the Firefox Addons store, or by clicking on [this link](https://addons.mozilla.org/en-CA/firefox/addon/keepassxc-browser/). Once you've got the browser extension installed, you need to open KeePassXC, and navigate to Tools &#x2013;> Settings &#x2013;> Browser Integration. Check "*Enable Browser Integration*" and then use the check mark to enable interaction with the browser extension on your respective browser. Then, before you start your browser, you can start KeePassXC and it will succesfully connect to the browser extension, and auto fill your forms on websites. 


<a id="org51e7dfa"></a>

# You did it!

If you've followed the instructions correctly, you should now be able to start KeePassXC, enter a password, launch your browser, and have all the usernames and passwords on all of your websites filled out automatically. This ensures that all of your passwords are secure, and hosted locally on your machine with no chance that they get stolen in data breach. You can rest easy knowing that all of your accounts are safe, and that someone named *H4CK3R11026* won't gain access to all of your precious accounts just because you used the same password on a forum back in 2010. 


# Table of Contents

1.  [Installing KeePassXC](#org3b52d73)
    1.  [Ubuntu/Debian](#orgf4a3eae)
    2.  [Fedora/CentOS/](#orgf68b2d4)
    3.  [Arch/Manjaro](#orgbc7b3e5)
    4.  [OpenSUSE](#org50119a9)
2.  [Creating a database](#org4d0af46)
    1.  [Encryption Settings](#org4971603)
    2.  [Password Creation](#org58ab6da)
3.  [Creating an Entry](#orgde89e99)
4.  [Using the Browser Extension](#org2a795fd)
5.  [You did it!](#org51e7dfa)
