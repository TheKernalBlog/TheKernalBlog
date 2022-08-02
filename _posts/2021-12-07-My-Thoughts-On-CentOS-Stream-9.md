---
published: true
---
The time has finally come, the CentOS that you once knew is dead. While there are equivalent projects like Rocky or Alma Linux, the EOL for CentOS 8 is fast approaching at the end of the year. The CentOS team announced CentOS Stream, and while I understood their vision, I disagreed with them abandoning the model that has brought them so much success in the server and enterprisr world. CentOS stream has finally come out, and I decided to try it out in a Virtual Machine with GPU-Passthrough, so it is equivalent to running on real hardware. I am going to give my experience, what I liked, and what was bad about my experience. 

# Psuedo-Rolling Release 

CentOS Stream has seemed to have taken a weird choice when it comes to  the rolling-release model. When Stream was first announced, I thought it would act like Arch or OpenSUSE Tumbleweed, with one version that gets continually updated. Then I saw that this rolling release distro would have multiple versions, like Solus. I thought, "I get that, as long as they make it so that you can choose to upgrade to the newer versions whenever you want". You know what happened, they made it so that the only way that you can update from CentOS Stream 8 to CentOS Stream 9 is by re-installing. At this point, it would me much easier to move a CentOS Stream 8 server to Rocky Linux (not backed by RedHat) to the official RedHat sponsored CentOS Stream 9. 

# Desktop usage

While CentOS is not made for the desktop, there are many people, especially people who are experienced with RedHat that like to use CentOS for their desktop. I have to say, CentOS Stream 9 was great for regular desktop activities. I found PipeWire to be much more stable and easy to use than Pulseaudio. From my usage of CentOS 8 Stream with the GNOME desktop, ram usage has dropped about 25%, which I think has to do with the newer version of GNOME and the Linux kernel itself. I had no issues whatsoever other than the rather limited package count. I would almost be impressed if Fedora didn't exist and CentOS was actually made for desktops. 

# Server Usage

While I would argue that there are better Linux distro's for the server, I found the experience of using CentOS Stream 9 was quite pleasant. I only tried hosting a file and web server, but I found the process of installing, configuring, and running them very easy. However, the same could be said on about any version of Red Hat Enterprise Linux or CentOS. I think that despite not being binary-compattable with Red Hat, it is *almost* just as stable. You only really should update once every week or two, which is not bad. If you would like some newer software I would say that the more frequent updates and some stability are a good trade off. 

# Conclusion 

While others would say that CentOS Stream 9 is the worst thing since Snapcraft, I think that if we were to view CentOS Stream 9 in a vacum, we would think it is a great OS. The only problem is that they are getting rid of the CentOS that many of us knew for years. I think that Rocky Linux or AlmaLinux are your best bets if you want something that is close to the old CentOS, but I would encourage you to give the newer CentOS Stream a try.
