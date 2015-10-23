# Workstation
My web development environment using Laravel on Ubuntu 14.04.2

## Requirements

> sudo apt-get update

## LAMP Server

### Apache Server
> sudo apt-get install apache2

### PHP5
> sudo apt-get install php5 libapache2-mod-php5 php5-mcrypt

### MySQL
> sudo apt-get install mysql-server php5-mysql
>
> sudo mysql_secure_installation

### PHPMyAdmin
> sudo apt-get install phpmyadmin

### Composer
> curl -sS https://getcomposer.org/installer | php
>
> mv composer.phar /usr/local/bin/composer

### Apache and PHP Modules to activate
> sudo php5enmod mcrypt
>
> sudo a2enmod rewrite

### NodeJS
> sudo apt-get install --yes nodejs

### Sublime Text
> sudo add-apt-repository ppa:webupd8team/sublime-text-2
>
> sudo apt-get update
>
> sudo apt-get install sublime-text

Install Package Control in Sublime Text

> Open Sublime Text
>
> Go to View > Show Console
>
> Copy and past this code

```
import urllib2,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')
```

> Restart Sublime Text

### My personal Sublime Text snippets
* Emmet
* Laravel Blade Highlighter
* Git
* Brogrammer

> Setup
>Activate the UI theme and color scheme by modifying your user preferences file, which you can find using the menu item Preferences -> Settings - User in Sublime Text or by clicking cmd + , on a Mac.

Example settings
```
{
  "theme": "Brogrammer.sublime-theme",
  "color_scheme": "Packages/Theme - Brogrammer/brogrammer.tmTheme"
}
```
