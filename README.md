# Stury CakePHP

## What's this
My study...

## Memo
## Setting for your database
	$ mv ./app/config/database.php.default ./app/config/database.php
	$ vim ./app/config/database.php

### Change security salt value
	$ vim ./app/config/core.php
	$ Configure::write('Security.salt', 'DYhG93b0qyJfIxfs2guVoUubWwvniR2G0FgaC9mi');

Example:
	$ openssl sha1 hoge.txt
 
### Change security chipher seed
vim app/config/core.php
Configure::write('Security.cipherSeed', '76859309657453542496749683645');

Example:
	$ for i in {1..10}; do echo -n $RANDOM; done;echo "";
 
### Change template file expression.
	./cake/libs/view/view.php:157:	var $ext = '.ctp';
	./cake/libs/controller/controller.php:240:	var $ext = '.ctp';
	./cake/libs/controller/scaffold.php:106:	var $ext = '.ctp';
	./cake/tests/cases/libs/debugger.test.php:239:	 View::$ext = ".ctp"

But keep default include cakephp .ctp files.

## CakePHP Original README
CakePHP is a rapid development framework for PHP which uses commonly known design patterns like Active Record, Association Data Mapping, Front Controller and MVC. Our primary goal is to provide a structured framework that enables PHP users at all levels to rapidly develop robust web applications, without any loss to flexibility.

The Cake Software Foundation - promoting development related to CakePHP
http://cakefoundation.org/

CakePHP - the rapid development PHP framework
http://www.cakephp.org

Cookbook - user documentation for learning about CakePHP
http://book.cakephp.org

API - quick reference to CakePHP
http://api.cakephp.org

The Bakery - everything CakePHP
http://bakery.cakephp.org

The Show - live and archived podcasts about CakePHP and more
http://live.cakephp.org

CakePHP TV - screen casts from events and video tutorials
http://tv.cakephp.org

CakePHP Google Group - community mailing list and forum
http://groups.google.com/group/cake-php

#cakephp on irc.freenode.net - chat with CakePHP developers
irc://irc.freenode.net/cakephp
