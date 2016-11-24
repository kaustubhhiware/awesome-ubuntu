# what_to_do_ubuntu
A repository to take uninitiated open-source - curios people through the installation procedure for ubuntu 16.04 , as most of the current users have done. For freshers , with love.

I think all of us using Ubuntu based-systems like to thank a lot of people for introducing us to open-source . So, this is us just passing the knowledge :).For any queries , feel free to contact me via [mail](mailto:hiwarekaustubh@gmail.com) or drop a [message on Facebook.](http://facebook.com/kaustubhhiware)
<Google group or chat for this would be great ?!>

**Under progress**
# Why install Linux?

Read more about this .
Some points :

* Contribute what you want , change and distribute

* More power, less BS (You can choose whatever version , everthing changes dynamically.)

* You'll be delighted by each update , not hate them.

# Installation prep-talk

This guide will be majorly focoused on Ubuntu 16.04 , but is valid for a range of open-source OS's.
If users wish to install only a single OS, you may skip this part, but it wouldn't hurt to know.Majority of Ubuntu users prefer dual boot, that is installing Windows as well as Linux on the same computer.If the user wants to go for dual-boot, install Windows first.You might face a lot of unnecessary problems if you try to install Windows after Ubuntu.Most laptops coming with pre-installed Windows, so why loose a licensed product you've already paid for ?

## Choosing an OS

There are a lot of OS out there , so choose wisely.When booting into a liveUSB, it is safer to test the OS first, as some OS's won't respond to your keyboard or some other issues.(To add an image here , distributing users by their OS.)(Find what a guide if possible.)

## Installation Guide

Although this is uncommon, a backup is suggested. In my last few attempts, it has been observed that backing up the C: drive suffices , if you do not have enough memory. However, this may not be true in all cases. I've written an answer on [Quora](https://www.quora.com/How-can-I-dual-boot-Windows-7-and-Linux/answer/Kaustubh-Hiw%CE%B1re) for installation, complete with images.

## Post installation

You need to first update the current system using
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-get update
sudo apt-get upgrade
sudo apt-get dist-upgrade</pre>

**NOTE** : Unlike windows, you'll be able to install only one application at a time, simply because it locks the list for repositories to look for updates later.(Very crude explanation).

In the meanwhile, you might want to tweak your OS with these 2 :

* One click minimise :
`gsettings set org.compiz.unityshell:/org/compiz/profiles/unity/plugins/unityshell/ launcher-minimize-window true`

* time recursive search -
  `gsettings set org.gnome.nautilus.preferences enable-interactive-search false`

* Install all media related support :
  `sudo apt-get install ubuntu-restricted-extras`

* flashplayer  : Playing videos and gifs in firefox
`sudo apt-get install flashplugin-installer`
* linuxdcpp : Peer-to-peer file sharing network
  `sudo apt-get install linuxdcpp`

  While you install the rest, you can upload the required minimum.

* codecs - Essentials for media formats and zip formats:

    `
  sudo apt-get install ffmpeg gxine libdvdread4 icedax tagtool libdvd-pkg easytag id3tool lame libxine2-ffmpeg nautilus-script-audio-convert libmad0 mpg321 libavcodec-extra gstreamer1.0-libav
   p7zip-rar p7zip-full unace unrar zip unzip sharutils rar uudeview mpack arj cabextract file-roller
  `

* [Atom](https://codeforgeek.com/2014/09/install-atom-editor-ubuntu-14-04/) : A hackable open-source editor

* [Chrome](http://askubuntu.com/questions/79280/how-to-install-chrome-browser-properly-via-command-line): An awesome web browser, owing to its [extensions](#chrome).  

* synaptic : package manager `sudo apt-get install synaptic`

* [sublimetext](http://tipsonubuntu.com/2015/03/27/install-sublime-text-2-3-ubuntu-15-04/) : A popular editor


* unity tweak tool and tweak tool  : Change the way your OS looks - another win for Linux
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-get gnome-tweak-tool
sudo apt-get install unity-tweak-tool</pre>

* vlc : `sudo apt-get install vlc`

* [appmenu](http://askubuntu.com/questions/122437/how-to-access-applications-menu-in-ubuntu-unity-desktop) - view all applications via a dropdown.
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-add-repository ppa:diesch/testing
sudo apt-get update
sudo apt-get install classicmenu-indicator</pre>

* [brightness indicator](http://www.omgubuntu.co.uk/2013/04/brightness-control-ubuntu) - control brightness via mouse.
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo add-apt-repository ppa:indicator-brightness/ppa
sudo apt-get update
sudo apt-get install indicator-brightness</pre>

# Git
 The most widely used version control system

`sudo apt-get install git`

* First time configuration:
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">git config --global user.name "your_username"
git config --global user.name "your_username"</pre>

 The next part is applicable if you work behind a proxy server.
  <pre>
 git config --global http.proxy http://10.3.100.207:8080
 git config --global https.proxy https://10.3.100.207:8080</pre>

# Python

Default 2.7.11+ is installed.

First of all , install [anaconda](https://www.continuum.io/downloads) - it makes your life easier. [Askubuntu answer](http://askubuntu.com/questions/505919/how-to-install-anaconda-on-ubuntu).

install pip -  `sudo apt-get install python-pip python3-pip`

following packages - beautifulSoup , tkinter , vpython ,twine,requests , mechanise, bs4,lxml
, django, __future__, yolog,matplotlib,scrapy,facepy

* yolog - beautifies git logs ,run in folder with `yolog`

* thefuck - corrects your previous command [here](https://github.com/nvbn/thefuck#manual-installation)

* scrapy :  `pip install Scrapy`

 If you run into an error while installing cryptography, [RTD.](https://cryptography.io/en/latest/installation/#building-cryptography-on-linux)

* fuck you - ragekill processes [here](https://github.com/robotlolita/fuck-you)

Mongo[DB](https://www.howtoforge.com/tutorial/install-mongodb-on-ubuntu-16.04/)

see this for [visual](https://www.youtube.com/watch?v=vszmuxnBBd8)

# Opencv

[a guide](http://milq.github.io/install-opencv-ubuntu-debian/)

[another guide](http://milq.github.io/install-opencv-ubuntu-debian/)

java : http://www.oracle.com/technetwork/java/javase/downloads/index.html

sudo se commands approve hote hai
http://www.wikihow.com/Install-Oracle-Java-on-Ubuntu-Linux

ipython

guake terminal

geany

gimp - image manipulation

Kazam - record screen

netbeans

gparted -  partition mgmt

theme configuration - the name

sudo apt-get install ubuntu-wallpapers-* edgy-wallpapers feisty-wallpapers gutsy-wallpapers

java - http://askubuntu.com/questions/145748/how-to-compile-a-java-file

# Chrome

Themes for [chrome here](https://chrome.google.com/webstore/detail/bluegreen-cubes/iipbjjaibkibpabddphfcgbngfhhfkml).
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

* [Mixmax](https://chrome.google.com/webstore/detail/mixmax-email-tracking-tem/ocpljaamllnldhepankaeljmeeeghnid/related?hl=en) - Email tracking

* [Magic](https://chrome.google.com/webstore/detail/magic-actions-for-youtube/abjcfabbhafbcdfjoecdgepllmpfceif?hl=en) - Magic actions for youtube  -check it out , easier sound control

# Node.js apps
Server - side javascript for creating awesome webapps.
 Need to set proxy here! This is specific for Kharagpur again.
`
 npm config set proxy http://10.3.100.207:8080
 npm config set https-proxy http://10.3.100.207:8080
`

* [Awesome resources](https://github.com/sindresorhus/awesome-nodejs#command-line-apps)
