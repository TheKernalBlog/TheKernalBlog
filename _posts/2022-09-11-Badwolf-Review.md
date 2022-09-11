---
published: false
---
Your browser sucks. It's just the cold hard truth. Almost every modern browser is extremely slow, confusing, and privacy invasive. While there have been many attempts to create a usable and fast browser, almost all of them are based on Ungoogled Chromium or Firefox, which, while good for privacy, are incredibly bloated. I've searched far and wide for a browser that fits my needs without adding on too much unnecessary crap, and I think I may have found it. [Badwolf](https://hacktivis.me/projects/badwolf) is a WebKitGTK based, Suckless browser that's quick, standardized, and no-nonsense. So if you're interested in Badwolf, I'll give you some general pointers and facts about this one-of-a-kind browser.

# Installing

## Arch Linux

- Requires a AUR helper. I'm using Yay, but feel free to use any other helper you choose.

	yay -S badwolf-bin

## Fedora

	sudo dnf install badwolf

## OpenSUSE

- Install the [Community](https://software.opensuse.org/package/badwolf?search_term=Badwolf) package.

## Ubuntu/Debian

- Build the package from [source](https://hacktivis.me/releases/badwolf-1.2.1.tar.gz)

# Usage

![Badwolf1](/images/Badwolf.png)

Overall, Badwolf is extremely simple. Almost everything is done with a mouse, and most of the shortcuts should carry over from your previous experience with other browsers. However, there are a few keyboard shortcuts that aren't very natural or common. I've compiled a table with some of the ones that I've personally had trouble with, but all of the shortcuts are also available on the manpage if you're still confused.

| Action                         | Shortcut             |
| ---                            | ---                  |
| Go Back/forward in tab history | Ctrl-[ & Ctrl-]      |
| Go to the next/previous tab    | Alt-Right & Alt-Left |
| Focus on URL entry bar         | Ctrl-l               |
| Kill the current tab           | Alt-d                |

# Resource Usage

![Badwolf2](/images/BadwolfHtop.png)

Badwolf is very lightweight. More than any other browser that I've ever used. RAM usually stays around 80-100MB, with a few tabs open. But the most surprising thing you'll see if you more closely inspect the picture above, is that the CPU usage is **0%**. That's right. With some more tabs open, I've seen it get up to around 5%, but it never uses any more than that. It's truly remarkable how lightweight this browser is.

# Privacy

As promised on the webpage, there is absolutely no browser-level tracking, including telementary (Mozilla *cough* *cough*). But there's one thing that not every browser has the cojones to do, disabling Javascript by default, which does wonders to prevent cross site scripting attacks and general spying from your favorite tech Oligarc's. But no worries, if there's a website that really needs Javascript, you can turn it on using a convenient little button. There's also a button that turns off images, which doesn't do much to protect privacy, but may help in very niche cases.

# Some Drawbacks

It can't be all good. In order to make the browser as fast and compact as possible, it seems like there have been quite a few features of most browsers that've been thrown out entirely. For example,

### Web History

Badwolf has absolutely no web history. Which, admittedly, isn't that bad for most people, but may be of concern if for some reason you can't remember the URL's of the sites that you commonly visit.

### Cookies

Cookies are one of the main methods used by companies to track users. However, they also have a very viable use for logins and other info you like to save. As soon as you close a tab, all the cookies are destroyed. So get used to typing your username and password every time you want to login to any website.

### Adblock

Badwolf comes with absolutely no form of adblock. And due to the lack of extensions, any sort of adblocking is very difficult. You have to create a json config file full of manually added ad systems. It's not ideal.

# Conclusion

Badwolf is an amazing, fast, and unique browser. It may not be the thing for you, but it still fills its niche incredibly well. It's a browser, nothing more. And that no-nonsense approach is something that is needed now more than ever, in the current space full of dime-a-dozen bloated, slow, and feature packed browsers. If you are in the need of something fast, and can handle the drawbacks, I would highly recommend that you give Badwolf a try, and see what it's like to have a browser that doesn't suck.
