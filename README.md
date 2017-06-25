# awesome-ubuntu
:sunglasses:

A repository to take uninitiated open-source - curious people through the installation procedure for ubuntu 16.04 , as most of the current users have done. For freshers , with love.

I think all of us using Ubuntu based-systems like to thank a lot of people for introducing us to open-source . So, this is me just passing the knowledge :smile:.For any queries , feel free to contact me via [mail](mailto:hiwarekaustubh@gmail.com) or drop a [message on Facebook.](http://facebook.com/kaustubhhiware)
<Google group or chat for this would be great ?!>

**Proceeding towards proper release**
# Why install Linux?

Read more about this .
Some points :

* Contribute what you want , change and distribute

* More power, less BS (You can choose whatever version , everthing changes dynamically.)

* You'll be delighted by each update , not hate them.

# Installation prep-talk

This guide will be majorly focoused on Ubuntu 16.04 , but is valid for a range of open-source OS's.
If users wish to install only a single OS, you may skip this part, but it wouldn't hurt to know.Majority of Ubuntu users prefer dual boot, that is installing Windows as well as Linux on the same computer.If the user wants to go for dual-boot, install Windows first.You might face a lot of unnecessary problems if you try to install Windows after Ubuntu.Most laptops coming with pre-installed Windows, so why loose a licensed product you've already paid for ?

# Choosing an OS

There are a lot of OS out there , so choose wisely.When booting into a liveUSB, it is safer to test the OS first, as some OS's won't respond to your keyboard or some other issues.(To add an image here , distributing users by their OS.)(Find what a guide if possible.)

# Installation Guide

Although this is uncommon, a backup is suggested. In my last few attempts, it has been observed that backing up the C: drive suffices , if you do not have enough storage space. However, this may not be true in all cases. I've written an answer on [Quora](https://www.quora.com/How-can-I-dual-boot-Windows-7-and-Linux/answer/Kaustubh-Hiw%CE%B1re) for installation, complete with images.

# Post installation

You need to first update the current system using
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-get update
sudo apt-get upgrade
sudo apt-get dist-upgrade</pre>

[Create a hotspot in Ubuntu](http://askubuntu.com/questions/490950/create-wifi-hotspot-on-ubuntu).


**NOTE** : Unlike windows, you'll be able to install only one application at a time, simply because it locks the list for repositories to look for updates later.(Very crude explanation).


In the meanwhile, you might want to tweak your OS with these  :

* apt-fast :  A shellscript wrapper for apt-get and apt that drastically speeds up downloading of packages by downloading packages in parallel, with multiple connections per package.  
```
sudo add-apt-repository ppa:saiarcot895/myppa
sudo apt-get update
sudo apt-get -y install apt-fast 
```
During installation it will ask you to change number of connections for downloading, change it's value to any high value like 16.
Afterwards, use apt-fast instead of apt-get or apt.

* flux : It makes the color of your computer's display adapt to the time of day, warm at night and like sunlight during the day.
```
sudo add-apt-repository ppa:nathan-renniewaldock/flux
sudo apt-get update
sudo apt-get install -y fluxgui && fluxgui
```
    
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
* eiskaltdcpp : Alternative to linucdcpp
`sudo apt-get install eiskaltdcpp`
  While you install the rest, you can upload the required minimum.

* [Chrome](http://askubuntu.com/questions/79280/how-to-install-chrome-browser-properly-via-command-line): An awesome web browser, owing to its [extensions](#chrome).  Install the extensions you want while the rest is installed via apt-get.

* codecs - Essentials for media formats and zip formats:
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-get install ffmpeg gxine libdvdread4
 sudo apt-get install icedax tagtool libdvd-pkg
 sudo apt-get install easytag id3tool lame libxine2-ffmpeg
 sudo apt-get install nautilus-script-audio-convert libmad0
 sudo apt-get install mpg321 libavcodec-extra gstreamer1.0-libav
 sudo apt-get install  p7zip-rar p7zip-full unace unrar zip unzip
 sudo apt-get install  sharutils rar uudeview mpack arj cabextract file-roller</pre>.

 Mentioned in separate lines for ease of viewing. You may as well install all simultaneously.

**NOTE**: You will get a purple screen in your terminal to accept some terms and
 conditions while this installation. Press tab to switch between options.

* [tree](http://askubuntu.com/questions/431251/how-to-print-the-directory-tree-in-terminal) - View Directory tree in terminal as below :
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">
$ tree # or tree /path/to/folder
.
├── AndroidManifest.xml
├── java
│   └── com
│       ├── example
│       │   └── kaustubh
│       │       └── calculator
│       │           └── MainActivity.java
│       └── learning
│           └── kaustubh
│               └── calculator
│                   └── MainActivity.java
└── res
    ├── drawable
    ├── layout
    │   └── activity_main.xml
    ├── mipmap-hdpi
    │   └── ic_launcher.png
    ├── mipmap-mdpi
    │   └── ic_launcher.png
    ├── mipmap-xhdpi
    │   └── ic_launcher.png
    ├── mipmap-xxhdpi
    │   └── ic_launcher.png
    ├── mipmap-xxxhdpi
    │   └── ic_launcher.png
    ├── values
    │   ├── colors.xml
    │   ├── dimens.xml
    │   ├── strings.xml
    │   └── styles.xml
    └── values-w820dp
└── dimens.xml
</pre>
 Install with `sudo apt-get install tree`



* Get all the ubuntu wallpapers.Ever.
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-get install ubuntu-wallpapers-* edgy-wallpapers feisty-wallpapers gutsy-wallpapers</pre>


* [Atom](https://codeforgeek.com/2014/09/install-atom-editor-ubuntu-14-04/) : A hackable open-source editor with inbuilt markdown viewer.

* synaptic : package manager `sudo apt-get install synaptic`

* [sublimetext](http://tipsonubuntu.com/2015/03/27/install-sublime-text-2-3-ubuntu-15-04/) : A popular editor

 Another additions to sublime text would be [Package Control](https://packagecontrol.io/installation#st2) ,after which a [spacegray theme](https://github.com/kkga/spacegray) may be chosen.


* unity tweak tool and tweak tool  : Change the way your OS looks - another win for Linux
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-get install gnome-tweak-tool
sudo apt-get install unity-tweak-tool</pre>.

You can pair it up with theme configuration to customise colours.
You might as well experiment with [desktop environments](http://askubuntu.com/questions/65083/what-kinds-of-desktop-environments-and-shells-are-available).

* vlc : `sudo apt-get install vlc`

* [Foxit Reader](http://sourcedigit.com/20670-how-to-install-foxit-reader-in-ubuntu-using-terminal/) : A great pdf viewer for Linux

* [wine](http://ubuntuhandbook.org/index.php/2015/12/install-wine-1-8-stable-new-ppa/): Emulate few windows applications in ubuntu.

* [R and Rstudio](https://www.datascienceriot.com/how-to-install-r-in-linux-ubuntu-16-04-xenial-xerus/kris/)

* guake terminal: Drop down terminal `sudo apt-get install guake -y`

* geany - Awesome text editor with inbuilt terminal `sudo apt-get install geany`

* [gimp](http://ubuntuhandbook.org/index.php/2015/11/how-to-install-gimp-2-8-16-in-ubuntu-16-04-15-10-14-04/) - image manipulation

* Kazam - for screencasts

 <pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-add-repository ppa:sylvain-pineau/kazam
sudo apt-get update
sudo apt-get install kazam</pre>
* [gparted](http://ubuntuhandbook.org/index.php/2013/09/install-upgrade-gparted-0-16-2-in-ubuntu-13-04-12-04/) -  partition management
`sudo apt-get install gparted`

* [LaTeX](http://milq.github.io/install-latex-ubuntu-debian/) - making documents with links.(Crude)Ever seen those resume.pdf's with links ? LaTeX made them.

Some menu apps:
* [appmenu](http://askubuntu.com/questions/122437/how-to-access-applications-menu-in-ubuntu-unity-desktop) - view all applications via a dropdown.
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo apt-add-repository ppa:diesch/testing
sudo apt-get update
sudo apt-get install classicmenu-indicator</pre>

* [brightness indicator](http://www.omgubuntu.co.uk/2013/04/brightness-control-ubuntu) - control brightness via mouse.
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo add-apt-repository ppa:indicator-brightness/ppa
sudo apt-get update
sudo apt-get install indicator-brightness</pre>


## Chrome

Themes for chrome on [chrome webstore](https://chrome.google.com/webstore/detail/bluegreen-cubes/iipbjjaibkibpabddphfcgbngfhhfkml).
Some much needed extensions :

* [AdBlock](https://chrome.google.com/webstore/detail/adblock/gighmmpiobklfepjocnamgkkbiglidom) - stop stupid ads from reducing your productivity

* [Be Limitless](https://chrome.google.com/webstore/detail/be-limitless/jdpnljppdhjpafeaokemhcggofohekbp) - A Productivity tool to track your time on websites

* [Camera](https://chrome.google.com/webstore/detail/camera/hfhhnacclhffhdffklopdkcgdhifgngh) - a chrome app , if your laptop's camera can't be opened in any other way

* [Google dictionary](https://chrome.google.com/webstore/detail/google-dictionary-by-goog/mgijmajocgfcbeboacabfgobmjgjcoja) - Stuck on a word and every time need to search it ?
No more , just drag over the word and right click to know the meaning

* [Google Keep](https://chrome.google.com/webstore/detail/google-keep-chrome-extens/lpcaedmchfhocbbapmcbpinfpgnhiddi) - online note making app,synchronises with its android app

* [MakkhiChoose](https://chrome.google.com/webstore/detail/makkhichoose/gllmlkidgbagkcikijiljllpdloelocn) - For your online shopping expeditions.Keeps track of a products's prize over
time , compares with other platforms for cheaper rates

* [PanicButton](https://chrome.google.com/webstore/detail/panicbutton/faminaibgiklngmfpfbhmokfmnglamcm) - You get more than what the name says - immediately bookmark all open tabs ,
to view later . With one click , minimise all your tabs , review with another click.

* [Pushbullet](https://chrome.google.com/webstore/detail/pushbullet/chlffgpmiacpedhhbkiomidkjlcfhogd) - Send messages over the net , to your friends , or to yourself instead of
bookmarking it and forgetting it . Android app available.

* [Savefrom.net helper](http://en.savefrom.net/1-how-to-download-youtube-video/) - download video tutorials , playlists , etc within minutes -
	downloads multiple files at a time with consistent speed

* [Tatkal ticket now](https://chrome.google.com/webstore/detail/tatkal-ticket-now/konojmimochobcfkmnamhlhnpiofplkm) - Tatkal reservations ? Check PNR within seconds -done.

* [UglyEmail](https://chrome.google.com/webstore/detail/uglyemail/ldgiafaliifpknmgofiifianlnbgflgj) - Know who tracks your mail- tracked mails have a eye icon on their right.

* [Video speed controller](https://chrome.google.com/webstore/detail/video-speed-controller/nffaoalbilbmmfgbnbgppjihopabppdk) - The world is not fast enough for you?- view videos across a lot of
platforms , at speeds higher than 2x , without audio distortion

* [Mixmax](https://chrome.google.com/webstore/detail/mixmax-email-tracking-tem/ocpljaamllnldhepankaeljmeeeghnid/related?hl=en) - Email tracking

* [Magic](https://chrome.google.com/webstore/detail/magic-actions-for-youtube/abjcfabbhafbcdfjoecdgepllmpfceif?hl=en) - Magic actions for youtube  -check it out , easier sound control

## Git
 The most widely used version control system

`sudo apt-get install git`

* First time configuration:
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">git config --global user.name "your_username"
git config --global user.email "name@where.com"</pre>

 The next part is applicable if you work behind a proxy server.
  <pre>
 git config --global http.proxy http://10.3.100.207:8080
 git config --global https.proxy https://10.3.100.207:8080</pre>

## Python

Default 2.7.11+ is installed.

First of all , install [anaconda](https://www.continuum.io/downloads) - it makes your life easier. [Installation](http://askubuntu.com/questions/505919/how-to-install-anaconda-on-ubuntu).

install pip -  `sudo apt-get install python-pip python3-pip`

Install the following packages - beautifulSoup , tkinter , vpython ,twine,requests , mechanise, bs4 , lxml , ipython , django , __future__ , yolog , matplotlib , scrapy , facepy

with `pip install package_name` or `sudo -H pip install package_name` unless specifically mentioned.

* [yolog](https://github.com/karandesai-96/yolog) - beautifies git logs ,run in folder with `yolog`

* [thefuck](https://github.com/nvbn/thefuck#manual-installation) - corrects your previous command.

* scrapy :  `pip install Scrapy`

 If you run into an error while installing cryptography, [RTD.](https://cryptography.io/en/latest/installation/#building-cryptography-on-linux)

* [fuck you](https://github.com/robotlolita/fuck-you) - ragekill processes.

* Mongo[DB](https://www.howtoforge.com/tutorial/install-mongodb-on-ubuntu-16.04/)

* see this for [visual](https://www.youtube.com/watch?v=vszmuxnBBd8)


## Android studio and Java

You need to install the compatible version of java first.
<pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
sudo apt-get install oracle-java8-set-default</pre>

* netbeans - An IDE for java


Another alternative links for java : [Link1](http://www.oracle.com/technetwork/java/javase/downloads/index.html) [Link2](http://www.wikihow.com/Install-Oracle-Java-on-Ubuntu-Linux
) [Link3](https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04).

Follow this [answer on askubuntu](http://askubuntu.com/questions/634082/how-to-install-android-studio-on-ubuntu) for installing android studio.


## Customising terminal
Although there may be options like zsh, I'd prefer [fish](https://fishshell.com/), a user friendly command-line shell. Installation guides :
 [Link1](https://hackercodex.com/guide/install-fish-shell-mac-ubuntu//)
 [Link2](http://www.makeuseof.com/tag/x-reasons-install-fish-shell/).
 
 Once you've installed and configured basic fish, you would want a plugin manager like [fisherman](https://github.com/fisherman/fisherman/wiki) .
 Some interesting [plugins](https://github.com/jbucaran/awesome-fish).
 
 
## Node.js apps
Server - side javascript for creating awesome webapps.
[Installation guide](http://www.hostingadvice.com/how-to/install-nodejs-ubuntu-14-04/).
 Need to set proxy here! This is specific for Kharagpur again.


 <pre style="background: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); padding: 5px 10px;">npm config set proxy http://10.3.100.207:8080
npm config set https-proxy http://10.3.100.207:8080</pre>


* [Awesome resources](https://github.com/sindresorhus/awesome-nodejs#command-line-apps)

## Opencv
 Essential for image processing.

Installation guides :
[Link1](http://milq.github.io/install-opencv-ubuntu-debian/) [Link2](http://milq.github.io/install-opencv-ubuntu-debian/).

[Tutorials](http://docs.opencv.org/3.0-beta/doc/py_tutorials/py_tutorials.html).


## Sample

I've added relevant commands from my bash_history in a file here. Let's see if a script is needed to automate all of setup.

Have a suggestion ? Make an issue about it.
