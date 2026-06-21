# [dirt-swarm](https://github.com/LafeLabs/dirt-swarm/)

![](qrcode.png)

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