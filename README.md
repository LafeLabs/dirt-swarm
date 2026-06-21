# [dirt-swarm](https://github.com/LafeLabs/dirt-swarm/)

![](qrcode.png)

SETI is pointed the wrong way. 

Dirt swarm is an autonomous swarm of web servers which gather information about the living earth and stream it across the swarm to analyze and understand and to ultimately become one with the living Earth.

The Dirt Swarm collects data on soil, air, water, living systems, machines, and electromagnetic fields via Python, connects with it via a web interface for swarm control of how the data flow grows the network. The network will spread media which builds more servers and adds more mesh nodes which host more servers. Servers  are built to be off grid with solar, wind, water, bike drive as much as possible.  

Servers are built to be mobile and always taking data, moving around, growing the network. 

Dirt swarm is a self-replicating set of files which connect a Python back end to a web-based front end. This system runs Apache and PHP and has no server-side JavaScript. PHP moves data between the Python back end and the JavaScript front end. The [P5.js](https://p5js.org/) JavaScript library provides real time interaction with humans. Code is all edited in situ using applications built on PHP and syntax highlighting with [ace.js](https://ace.c9.io/).  

The whole system is small enough to fit on a Floppy disk and can run on essentially anything that can run a web server and PHP, which is now everything. This is intended to be scaled primarily on waste-stream sourced hardware and on peoples existing machines, with no new hardware being bought for it.

There is no database on the back end. The PHP talks to the Python via [bridge.php](bridge.php), with JSON passed in both directions, and plots passed from Python back to HTML via base 64 encoding. This framework has prototype examples on the Python side of the minimum required to get started, but is designed for maximum flexibility on the Python side. Python can connect the front end web interface with all of the things Python now does which include a very wide range of applications now, but we in particular focus on control of physical scientific instruments, and analysis of scientific data, both of which have become universally covered by well-suppoerted open source Python libraries.

A major purpose of the file set presented here is to build a pipeline with the absolute minimum number of parts between Python, which can do literally everything in tech now and the Web, which remains a very effective way for machines to interact with humans. And we keep p5js as part of everything since that makes the JavaScript required for real time human interface to be easy and simple and well-documented.



## Windows Server:

 - [xampp for easy install on  windows or mac](https://www.apachefriends.org/download.html)

## Install code on linux:

```
sudo apt update
sudo apt install apache2 -y
sudo apt install php libapache2-mod-php -y
cd /var/www/html
sudo rm index.html
sudo apt-get install curl
sudo curl -o replicate-file-set.php https://raw.githubusercontent.com/LafeLabs/dirt-swarm/refs/heads/main/replicate-file-set.php
cd ..
sudo chmod -R 0777 *
cd html
php replicate-file-set.php
sudo chmod -R 0777 *
ln -s /var/www/html ~/Desktop/html
```

## [self-replicating php script](https://github.com/LafeLabs/dirt-swarm/blob/main/replicate-file-set.php)

## web files

 - [branch.html](branch.html)
 - [data.html](data.html)
 - [delete-files.html](delete-files.html)
 - [edit-files.html](edit-files.html)
 - [files.html](files.html)
 - [icon.html](icon.html)
 - [index.html](index.html)
 - [live-web-instrument.html](live-web-instrument.html)
 - [plots.html](plots.html)
 - [qrcode.html](qrcode.html)
 - [readme.html](readme.html)
 - [text.html](text.html)

## php files

 - [branch.php](branch.php)
 - [bridge.php](bridge.php)
 - [delete-branch.php](delete-branch.php)
 - [delete-file.php](delete-file.php)
 - [generate-file-set.php](generate-file-set.php)
 - [list-branches.php](list-branches.php)
 - [list-files.php](list-files.php)
 - [load-file.php](load-file.php)
 - [replicate-file-set.php](replicate-file-set.php)
 - [replicate-local-file-set.php](replicate-local-file-set.php)
 - [save-file-get.php](save-file-get.php)
 - [save-file.php](save-file.php)
 - [save-png.php](save-png.php)
 - [upload-image.php](upload-image.php)

## markdown files

 - [README.md](README.md)
 - [data.md](data.md)
 - [files.md](files.md)
 - [plots.md](plots.md)

## json files

 - [file-set.json](file-set.json)
 - [icon.json](icon.json)
 - [instrument-control.json](instrument-control.json)
 - [social-data.json](social-data.json)
 - [text.json](text.json)

## python files

 - [camera.ipynb](camera.ipynb)
 - [data_feed.ipynb](data_feed.ipynb)
 - [icon.ipynb](icon.ipynb)
 - [icon.py](icon.py)
 - [jupyter.ipynb](jupyter.ipynb)
 - [live_web_instrument.ipynb](live_web_instrument.ipynb)
 - [live_web_instrument.py](live_web_instrument.py)
 - [text.py](text.py)