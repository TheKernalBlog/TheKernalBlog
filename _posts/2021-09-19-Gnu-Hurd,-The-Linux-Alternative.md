---
published: true
---
If you have been following alternative operating systems for a while, there is a good change that you have heard of Hurd. It has been in development since before Linux, and yet it is still not stable. This kernel with a super cool logo is super powerful. I am going to tell you where you can get it, why you might want to check it out, and some of it’s drawbacks. 

# Where can I get it? 

Currently, the two only ways that you can get it is with Debian or Guix. We all know Debian, who have done work with the Linux, FreeBSD, and now Hurd kernel. It <a href="https://cdimage.debian.org/cdimage/ports/11.0/hurd-i386/">Has A Downloadable iso</a> with Gnu Hurd. Gnu Guix you might not have heard of before, it is made by the Gnu foundation, consists of only free software, and uses the Guix package manager which is based off of Nix. Currently Guix supports the Linux-Libre kernel, and the Hurd kernel, but eventually support for the Linux kernel will be dropped entirely. Much like Debian, Guix has a iso available for download <a href="https://guix.gnu.org/en/download/latest/">Right Here.</a>  

# Why should I use it?

Gnu Hurd has some amazing features. The main feature is that it uses a modular design to separate all of the aspects of the kernel into separate components. This means that you can substitute and change aspects of the kernel without having to rewrite everything, or even reboot your machine. It is designed to be easily swapped out and changed. Plus, in Gnu fashion, all of the components are 100% free, optimizing user freedom and privacy. 

# Why shouldn’t I use it? 

One of the main reasons that Hurd is disregarded is that development takes SO LONG. Gnu Hurd has been around for a very long time, and is still in active development. It likely won’t be out of active development for another 5-10 years. Plus, there are many utilities that will just not work with Gnu Hurd, for example Systemd. It is in an unfinished state and has been for decades. 

# Conclusion 

Gnu Hurd is an interesting project that is super cool and has a lot of potential. I personally, would not use it simply because there seems to be little support for it and it is still not out of active development. I would implore anyone interested in the structure and features of Hurd to check it out, as I truly believe it to have a lot of potential.
