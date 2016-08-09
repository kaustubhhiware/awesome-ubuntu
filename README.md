# what_to_do_ubuntu
A repository to take uninitiated open-source - curios people through the installation procedure for ubuntu 16.04 , as most of the current users have done. For freshers , with love.

I think all of us using Ubuntu based-systems like to thank a lot of people for introducing us to open-source . So, this is us just passing the knowledge :).For any queries , feel free to contact me via [mail](mailto:hiwarekaustubh@gmail.com) or drop a [message on Facebook.](http://facebook.com/kaustubhhiware)
<Google group or chat for this would be great ?!>

Please note: This README will be update daily. So, It would be better to share your ideas through 
issues, rather than PR's. Pull requests would be great after 20th July, till then please bear with me.

Extension

# Why install Linux?

Read more about this . 
Some points : 
=>Contribute what you want , change and distribute

=>More power , less BS (You can choose whatever version , everthing changes dynamically.)

=>You'll be delighted by each update , not hate them.

=>Find the quora answer by the professor whose 5-yr old daughter explains OS ;)

# Installation prep-talk

This guide will be majorly focoused on Ubuntu 16.04 , but is valid for a range of open-source OS's.
If users wish to install only a single OS, you may skip this part, but it wouldn't hurt to know.Majority of Ubuntu users prefer dual boot, that is installing Windows as well as Linux on the same computer.If the user wants to go for dual-boot, install Windows first.You might face a lot of unnecessary problems if you try to install Windows after Ubuntu.Most laptops coming with pre-installed Windows, so why loose a licensed product you've already paid for ?

## Choosing an OS

There are a lot of OS out there , so choose wisely.(To add an image here , distributing users by their OS.)(Find what a guide if possible.)

## Installation Guide

Although this is uncommon, a backup is suggested. In my last few attempts, it has been observed that backing up the C: drive suffices , if you do not have enough memory. However, this may not be true in all cases. 

## After installing

You need to first update the current softwares using
`
sudo apt-get install ubuntu-restricted-extras
`

Install all media related support :
`
sudo apt-get install ubuntu-restricted-extras
`
* linuxdcpp

* chromium

* vlc

* restricted extras

* https://www.sublimetext.com/ - a [guide](http://tipsonubuntu.com/2015/03/27/install-sublime-text-2-3-ubuntu-15-04/
).

* unity tweak tool and tweak tool ubuntu-tweak

>one click minimise - http://www.2daygeek.com/top-important-things-to-do-after-installing-ubuntu-16-04-lts-xenial-xerus/#

`sudo apt-get install flashplugin-installer`

>time recursive search - http://www.noobslab.com/2016/04/important-20-tweaksthings-to-do-after.html

codecs - Terminal Command:
`
sudo apt-get install ffmpeg gxine libdvdread4 icedax tagtool libdvd-pkg easytag id3tool lame libxine2-ffmpeg nautilus-script-audio-convert libmad0 mpg321 libavcodec-extra gstreamer1.0-libav
`

`
sudo apt-get install p7zip-rar p7zip-full unace unrar zip unzip sharutils rar uudeview mpack arj cabextract file-roller
`
* appmenu - view all applications via a dropdown [here](http://askubuntu.com/questions/122437/how-to-access-applications-menu-in-ubuntu-unity-desktop).

# DC

DC stands for direct connect . You'll need this if you have a hub at your college.You might come over various ways to do this , but the best way is also the easiest : 
`
sudo apt-get install linuxdcpp
`
# Git and Github

# Python 

First of all , install anaconda - it makes your life easier
< link !>

install pip -  `python get-pip.py`

using pip - `pip install -U pip setuptools`

following packages - beautifulSoup , tkinter , vpython ,twine,requests , mechanise, bs4,lxml
, django, __future__, yolog

*yolog - beautifies git logs ,run in folder with `yolog`

see this for [visual](https://www.youtube.com/watch?v=vszmuxnBBd8)

# Opencv

[a guide](http://milq.github.io/install-opencv-ubuntu-debian/)
[another guide](http://milq.github.io/install-opencv-ubuntu-debian/)

# Chrome 

Some much needed extensions :

* AdBlock - stop stupid ads from reducing your productivity
 
* Be Limitless - A Productivity tool to track your time on websites

* Camera - a chrome app , if your laptop's camera can't be opened in any other way

* Chime - Notification manager for all your accounts

* Google dictionary - Stuck on a word and every time need to search it ?
No more , just drag over the word and right click to know the meaning

* Google Keep - online note making app,synchronises with its android app

* MailTrack for Gmail - the name says it all.Track when people recieve your mail

* MakkhiChoose - For your online shopping expeditions.Keeps track of a products's prize over 
time , compares with other platforms for cheaper rates

* PanicButton - You get more than what the name says - immediately bookmark all open tabs ,
to view later . With one click , minimise all your tabs , review with another click.

* Pushbullet - Send messages over the net , to your friends , or to yourself instead of 
bookmarking it and forgetting it . Android app available.

* Savefrom.net helper - download video tutorials , playlists , etc within minutes - 
	downloads multiple files at a time with consistent speed

* Tatkal ticket now - Tatkal reservations ? Check PNR within seconds -done.

* UglyEmail - Know who tracks your mail- tracked mails have a eye icon with them
//add image later

* Video speed controller - The world is not fast enough for you?- view videos across a lot of 
platforms , at speeds higher than 2x , without audio distortion

# TODO : 
(shifted to contributing.md)

remove with : sudo apt-get remove unwanted_name

# References : 

* [dc](http://askubuntu.com/questions/569054/how-to-install-dc-on-ubuntu-14-04)
* [Also dc](https://ubuntuforums.org/showthread.php?t=193984)

Later add:


>python preinstalled on ubuntu 16

>java : http://www.oracle.com/technetwork/java/javase/downloads/index.html

sudo se commands approve hote hai
http://www.wikihow.com/Install-Oracle-Java-on-Ubuntu-Linux

after downloading jre , do 
sudo cp Downloads/jre_file /usr/local/java

# Newer, update kar

adding themes - download whatever you want theme

* all the wallpapers .ever.
`
 sudo apt-get install ubuntu-wallpapers* 
`

https://www.youtube.com/watch?v=9pntzL-S_PE

ipython

guake terminal

geany 

gimp - image manipulation
`

 sudo apt-get install gimp gimp-data gimp-plugin-registry gimp-data-extras

`

Kazam - record screen

netbeans

gparted -  partition mgmt

theme configuration - the name

theme for chrome - https://chrome.google.com/webstore/detail/bluegreen-cubes/iipbjjaibkibpabddphfcgbngfhhfkml

git - preinstalled at this point
config - https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-16-04
proxy -http://stackoverflow.com/questions/783811/getting-git-to-work-with-a-proxy-server


> opencv install : 
http://milq.github.io/install-opencv-ubuntu-debian/


synaptic package manager : sudo apt-get install synaptic

references:
http://www.webupd8.org/2016/04/things-to-do-after-installing-ubuntu-1604-lts-xenial-xerus.html
http://www.omgubuntu.co.uk/2016/04/10-things-to-do-after-installing-ubuntu-16-04-lts
http://ubuntuhandbook.org/index.php/2016/05/install-ubuntu-tweak-in-ubuntu-16-04/
synaptic - http://www.tecmint.com/things-you-mostly-need-to-do-after-installing-ubuntu-16-04/4/

java - http://askubuntu.com/questions/145748/how-to-compile-a-java-file
