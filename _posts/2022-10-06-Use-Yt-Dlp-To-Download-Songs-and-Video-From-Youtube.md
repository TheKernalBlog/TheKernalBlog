---
published: true
---
Youtube is the defacto place for video on the internet. There are other video hosting platforms, but none have even come close in popularity, profitability, or ease of use. Youtube is an essential pillar in the modern internet. However, it's owned by Google. There are many privacy concerns, along with inescapable adds and an insane amount of bloat. So, in response, people have started making various back-ends and clients. However, by far, the best option is to simply download the video files to be watched locally and offline. That's where yt-dlp comes in. yt-dlp is a package that downloads Youtube videos, extremely quickly and efficiently. And so, I'm going to show to install, and use yt-dlp, while providing a handy bash script that makes using yt-dlp a breeze.

# Installing yt-dlp

Depending on what distro you use, one of these commands into your terminal.

## Ubuntu/Debian

	sudo apt install yt-dlp ffmpeg

## Fedora/CentOS/Rocky

	sudo dnf install yt-dlp ffmpeg

## Arch/Manjaro

	sudo pacman -S yt-dlp ffmpeg

# Using yt-dlp

yt-dlp, at its core, is very simple. However, due to the considerable amount of audio and video formats provided, there's a few flags you have to memorize. Here are some of the commands for different formats.

## mp3

	yt-dlp -f 18 -x --audio-format mp3 ***LINK***

### ogg

	yt-dlp -f 18 -x --audio-format ogg ***LINK***

### flac

	yt-dlp -f 18 -x --audio-format flac ***LINK***

### mp4

	yt-dlp -f 18 ***LINK***

### webm

	yt-dlp ***LINK***

# Automating with a script

![YTD](/images/YTD.png)

While you definitely can write out the entire command every time you want to download a file, I find it extremely convenient, especially when dealing with music, to have a useful little simple shell script instead. So, with my limited knowledge, I wrote one. It's fully POSIX compliant and only 25 lines long.

```#!/bin/sh

echo "Enter the youtube link"
read link

echo "Would you like to download audio or video? Enter 1 for video and 0 for audio"
read va

if [ $va -eq 0 ]; then
cd ~/Music
echo "What audio format would you like? (mp3, ogg, flac)"
read aformat

yt-dlp -f 18 -x --audio-format $aformat $link

else

	cd ~/Videos
	echo "What video format would you like (mp4 or webm) "
	read vformat
	if [ $vformat = 'mp4' ]; then
		yt-dlp -f 18 $link
	else
		yt-dlp $link
	fi

fi
```

You can just copy-paste that into a file in your *~/.local/bin*, or, if you're weird, you can grab it from my [Github](https://github.com/TheKernalBlog/ytd).

# Conclusion

Now, you can download Youtube videos directly onto your hard drive to enjoy at your leisure. yt-dlp is simply, a better way of using Youtube. There's no fuss, no buffering, and best of all, no adds! You can download anything and everything. So go, build your music playlist, watch your favorite video essays, and do it all without all of Google's shittyness.
