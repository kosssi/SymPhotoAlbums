SymPhotoAlbums
==============

It's a simple gallery photos used symfony2.1.

## Installation

``` bash
git clone https://github.com/kosssi/SymPhotoAlbums.git
cd SymPhotoAlbums
cp app/config/parameters.yml.dist app/config/parameters.yml
curl -s http://getcomposer.org/installer | php
php composer.phar update friendsofsymfony/user-bundle
php composer.phar install
php app/console doctrine:database:create
php app/console doctrine:schema:create
```

## Lancer un serveur

``` bash
curl -L http://github.com/downloads/benja-M-1/symfttpd/symfttpd.phar 2> /dev/null > symfttpd.phar
php symfttpd.phar spawn -p 1872
```

## Prérequis pour mac

``` bash
sudo port -d selfupdate
sudo port install php5 +fastcgi
sudo port install php5-eaccelerator
sudo port install php5-exif
sudo port install php5-gd
sudo port install php5-gettext
sudo port install php5-iconv
sudo port install php5-imagick
sudo port install php5-mbstring
sudo port install php5-mcrypt
sudo port install php5-openssl
sudo port install php5-sqlite
sudo port install php5-xmlrpc
sudo port install php5-xsl
sudo port install php5-zip
sudo port install php5-posix
sudo port install lighttpd

cd /opt/local/etc/php5/
sudo cp php.ini-production php.ini
```