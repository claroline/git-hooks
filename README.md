# A collection of Git Hooks for Claroline Connect

pre-commit : One pre-commit to rule them all.
pre-commit-phpcs : Run PHP_CodeSniffer on all your PHP files to be commited. (Depends on php-cs-fixer)
pre-commit-jshint : Run JSHint on all your JavaScript files to be commited. (Depends on jshint)
pre-commit-image-optimize : Run pngcrush and jpegtran on your PNG files and JPG files to be commited. (Depends on pngcrush and jpegtran)
pre-commit-phpunit : Run PHPUnit. (Depends on PHPUnit)

## Installing

Instructions are for installing on an Ubuntu/Debian based system.

### Install php-cs-fixer

```` bash
sudo curl http://get.sensiolabs.org/php-cs-fixer.phar -o php-cs-fixer
sudo chmod a+x php-cs-fixer
sudo mv php-cs-fixer /usr/local/bin/php-cs-fixer
````
### Install jshint

```` bash
sudo apt-get install nodejs
sudo npm install -g jshint
````

### Install pngcrush and jpegtran

```` bash
sudo apt-get install pngcrush
sudo apt-get install libjpeg-progs
````

### Install phpunit

```` bash
wget https://phar.phpunit.de/phpunit.phar
chmod +x phpunit.phar
sudo mv phpunit.phar /usr/local/bin/phpunit
```` bash

## Usage

RTFM : [Installing git hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks)

The hooks are all stored in the hooks subdirectory of the Git directory. In most projects, that’s .git/hooks, so basicly copy all the needed hooks into your .git/hooks directory and make sure they are executable.