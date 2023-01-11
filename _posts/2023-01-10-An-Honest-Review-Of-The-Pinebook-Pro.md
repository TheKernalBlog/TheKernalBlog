---
published: true
---

![IMAGE](/images/Pinebok.png) 

# Introduction 

For a couple months, I've been using a fairly old, underpowered Acer laptop as my daily driver. With only 2 CPU cores, and less than 2GB of RAM, it was not the best computer in the world. I was fairly content, but recently during Christmas,  I was gifted a Pinebook pro. The Pinebook pro is the Linux communities answer to the Macbook, with a small price tag, sleek design, and a Linux OS pre-installed. And now that I've had the time to properly adjust to the Pinebook, I feel like I have enough insight to give a real, unbiased review of this unique computer. 

# Hardware 

For the price, the Pinebook pro has fairly exceptional hardware. It has 6 CPU cores, 4GB of RAM, and a surprisingly great 4 core GPU. 

## Display 

The display is amazing. I have yet to find another laptop of this price range, with quality hardware, that has a display this nice. It's a 14 inch HD 1920x1080 panel, with great color quality better than my former 500$ Dell laptop. 

## Keyboard 

The keyboard is also excellent. It has a nice, firm, tactile feel that doesn't make too much noise. I've noticed that once in a blue moon, a character will be typed twice, when I only hit the key once. But, there is a chance that that's just user error. 

## Trackpad 

The trackpad, while not awful, is not up to the same standards as the display or keyboard. It has a weirdly rough feel, but still feels inaccurate. It boasts multi-finger gestures, but doesn't seem to integrate with the default KDE environment. And worst of all, far too often, it will double/tripple click when you only touch it once.

## Speakers 

The speakers are fairly nice. Not amazing, but defiantly better than a standard Smartphone or Chromebook. It's got a nice balanced sound, and very little audio distortion. However I have noticed that they don't get very loud.  

## Battery 

This is the only piece of hardware that really bothers me. The battery lasts 4-5 hours, but it takes **forever** to charge. You need to hook it up for up to 3 hours to get it up to a full charge. If you like to travel around and use your laptop without a charger, I'm not sure the Pinebook is for you. 

# Software 

## Manjaro

I was extremely disappointing with the default OS. Manjaro is barely stable on x86 processors, and it's a ticking time bomb on ARM. I was only able to use Manjaro for a couple hours before it broke U-boot, and bricked my machine. I had to use a separate laptop to flash my SD card with Armbian, take the laptop apart, and switch a tine little switch to disable EMMC booting. 

I'd love to  use Manjaro. It has the absolute best hardware support for the Pinebook Pro, and it's fairly speedy and customizable, but sadly, it's just too unreliable for daily work. 

## U-Boot

U-Boot is the bootloader for the Pinebook Pro. And honestly, it's just kind of bad. There's no boot screen, no configuration options, and if it breaks you have to switch off the EMMC before you can even boot off of a USB or SD card. I would really like to see some improvements. But in the meantime, I'd urge anyone with a Pinebook Pro to install [Tow Boot](https://tow-boot.org/). It fixes a lot of the problems with U-Boot by adding an actual user interface, and multiple boot modes. There's really no reason not to use it. 

# Final Thoughts 

The Pinebook pro is pretty great. You get high-end hardware for the same price as a Chromebook. There are quite a few hiccups, as you would expect with completely community sourced software, but as is the case with all open sourced projects, it's only going to get better with time. I would not recommend the Pinebook Pro if you don't have at least intermediate Linux knowledge. It's not perfect, but hey, it's better than anything Apple's put out in 15 years. 