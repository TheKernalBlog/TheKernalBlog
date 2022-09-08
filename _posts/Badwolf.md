Your browser sucks. It's just the cold hard truth. Almost every modern browser is extremely slow, confusing, or privacy invasive. And while there have been many attempts to make a usable and fast browser, almost all of them are based on Ungoogled Chromium or Firefox, which, while good for privacy, are incredibly bloated. I've searched far and wide for a browser that fits my needs without adding on too much unnececary crap, and I think I may have found it. [Badwolf](https://hacktivis.me/projects/badwolf) is a WebKitGTK based, Suckless browser that's quick, standardized, and no-nonsense. If you're interested in Badwolf at all, I'll show you how you can install and use the Badwolf web browser, while giving my general opinion along the way.

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

Overall, Badwolf is extremely simple. Almost everything is done with a mouse, and most of the shortcuts should carry over from your previous experience with other browsers. However, there are a few keyboard shortcuts that aren't very natural or common. I've compiled a table with some of the ones that I've personally had trouble with, but all of the shortcuts are also available on in the manpage if you're still confused.

| Action                         | Shortcut           |
| ---                            | ---                |
| Go Back/forward in tab history | Ctrl-[ & Ctrl-]    |
| Go to the next/previous tab    | Alt-Right Alt-Left |
| Focus on URL entry bar         | Ctrl-l             |
