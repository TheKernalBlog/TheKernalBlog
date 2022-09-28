---
published: false
---
If you care about privacy, want some addons, and a generally fast and lightweight browsing experience, you probably use Firefox, or one of the many forks. But Firefox, like many other modern browsers has become increasingly bloated and inefficient to control with a keyboard. As a result, people have been switching over to Qutebrowser and Surf. And while these are amazing browsers that I would definitely recommend, there's another option that fewer people consider.Using CSS and Web Extensions to can get the fast, keyboard centered browser of your dreams. Here's how. 

# Vim Input 

While I have recommended [Vim-Vixen](https://thekernal.xyz/2022/04/22/How-To-Go-Mouse-Free-On-Linux/) in the past, I have found another browser extension that one ups Vim Vixen by a long shot. [Tridactyl](tridactyl.xyz) brings the modal control from Vim straight to your web browser. You can move around the web page in normal mode, manage history, bookmarks, and tabs using command mode, and of course, input text in input mode. It truly is a game-changer that has made my browsing experience much more cohesive and efficient. 

You can install it like any other extension in the Mozilla Addons Store using the link below. 

[Click Me!](https://addons.mozilla.org/en-US/firefox/addon/tridactyl-vim/)

# CSS Theming

![PIC1](/images/FirefoxTheKernal.png)

Thanks to the expansive community of Firefox users, there are hundreds, even thousands of CSS themes available for use right now. For our purposes, a CSS theme with very few menu bars and maximum screen real estate is ideal. There are many 'One Liner' themes that put all browser options on a single bar. However, the [one I've chosen](https://github.com/aadilayub/firefox-i3wm-theme) is even more minimal, in an attempt to integrate nicely with i3 and dwm. 

## Enabling CSS Theming 

![PIC2](/images/AboutConfig.png)

In modern versions of Firefox, CSS theming is not enabled by default. In order to enable it, you have to go to the *about:config* page. You can ignore the warning, and in the bar at the top of the page, type, 

	toolkit.legacyUserProfileCustomizations.stylesheets

then click the box on the right so that it's set to 'true'. 

## Downloading the CSS theme 

Assuming that you have git installed, all you need to do is type this command in your terminal to clone the repository. 

	git clone https://github.com/aadilayub/firefox-i3wm-theme 

## Applying the CSS theme 

![PIC3](/images/AboutProfile.png)

In order to apply the theme, you first need to find your correct Firefox profile directory. While you could go fishing in your file system yourself, there's a much easier way. Simply go to *about:profiles* and copy the root directory on your default profile. Once you've done that, you must create another directory called 'chrome' where your userChrome.css file is going to go. Just copy this command into your terminal, to achieve just that. 

	midkr -p ~/.mozilla/firefox/PROFILE.profile/chrome

Now, all you need to do is copy the userChrome.css file over like so. 

	cp ~/firefox-i3wm-theme/userChrome.css ~/.mozilla/firefox/PROFILE.profile/chrome 

# Conclusion

Qutebrowser is a fine browser, and may even be better than Firefox for some users. However, Firefox has much better support and many more addons. If you're just a regular user, I'd stick with Firefox, and these two tools allow a seamless Vim + tiling window manager experience. So now, if you need a browser to scratch that particular itch, you don't have to go through the hassle of switching browsers. 
