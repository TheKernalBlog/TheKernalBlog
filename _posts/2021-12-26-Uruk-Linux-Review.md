---
published: true
---
Much like the French NuTyX, the chances are that if you are not from Iraq you have not heard of Uruk. Uruk is a Iraqui, 100% Libre Linux distro based on Trisquel. With many unique tools and an easy to use, stable base. I am going to go over my experience with the instillation, hardware support, desktop, pre-installed software, and the tools that come with it. 

# Instillation 

I found the install very easy. It uses the same calamaris installer that both Ubuntu and it's Trisquel base use. One thing that I really liked is that they checked the box for disk encryption, which is something that many people would not do otherwise. The install finished in around 20 minutes on my 500GB HHD, which is quite average. 

# Hardware Support 

Uruk follows the FSF guidelines for Free software. This obviously means that the hardware support is not going to be good, especially when it comes to Wifi and sound cards. But I'm sorry to say that your brand new Nvidea graphics card and Intel WiFI card won't work. 

# Desktop 

Uruk has two "flavors". They have an XFCE and Mate desktop. Both of them look nearly identical, with a MacOS-Like desktop look and the Masalla icon theme, which was created by one of the developers. I found both of them to be extremely responsive and fast, even when running in a VM with 2GB of RAM and 2 cores. So you can use it on your super old computers. 

# Pre-Installed software

Uruk comes installed with a lot of software that the average user would use. It has the 100% Libre Abrowser, great support for the disabled, the LibreOffice suite, and GIMP. Including all of the software that comes with your desktop environment of choice, you have access to faster and better software than almost any other Linux disto I've used. 

# Uruk tools 

Uruk has many tools that allow for better and easier software management, such as u-rpmi, u-src, and the package manager simulator. I am going to go over these tools and my experience with each. 

## u-rpmi 

Have you ever needed to install something and realized that while it is not available as a .deb package, it is available as a .rpm package. Uruk handles this perfectly, with u-rpmi. While there is no official .rpm repo for Uruk, by simply downloading a .rpm binary and running 

	u-rpmi filename.rpm 

The rpm will be installed on your system. It is really unique and one of my favorite gimmicks from any Linux distro. 

## u-src 

Installing software from source can be complicated, especially for a beginner. U-src allows you to just use one command and install any software from the source. You can simply download the source and install with 

	u-src package.tar.gz 

. This is also one great way to get any nonfree software on Uruk if you really need it. 

## Package manager simulator 

This is one of the most hyped up feature of Uruk. It allows you to simulate the commands of any popular package manager. You may be thinking, "How does that not create conflicts", but in reality, they still just use their one package manager with a different skin. You can use the commands for dnf, zypper, pacman, and apt, but in reality all of them are going to do the same thing. 

# Conclusion 

Uruk is a distro that I feel like more people should use. It has many cool features and quirks that make it one of the best Linux distro's I've tried out in a long time. It is perfect for new and experienced users alike. If you have any old old or home computers I would defiantly try it out.
