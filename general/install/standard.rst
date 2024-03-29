=====================
How To Intall Societo
=====================

This document explains about installation of Societo.

This is a simple document. If you want to get more detail information about Societo, please visit http://societo.org/documentation/

Requirements and Optionals
==========================

Requirements
------------

* A web server (we tested in Apache)
* PHP 5.3.2 or later
    * Required to enable PDO extension with MySQL driver
* MySQL 5.0 or later
    * Make sure your MySQL supports InnoDB (or InnoDB plugin)
    * Give privileges for creating / dropping / altering tables, and inserting / deleting / updating / selecting table data to your database user

Optional
--------

* PHP extension
    * XML
    * APC
    * mbstring or iconv (mbstring is recommended)
* Apache module
    * mod_rewrite module

Installation
============

NOTE: Installation from command line are not explained here. Visit http://societo.org/documentation/

1. Download and extract Societo package
---------------------------------------

Get a latest package from http://societo.org/

Packages are available in .zip format. You must get a compression tool for zip to extract.

(If you want to know about installation in Git version, please visit http://societo.org/documentation/)

After extract, and if you work it in your local machine, please upload the extracted package to your web server.

Last, set the document root to web/ directory in the extracted / uploaded Societo directory. If it is difficult, you can put a whole of the directory to your public HTML directory, but Societo doesn't support this situation.

2. Create database (you may skip this section if you already have)
------------------------------------------------------------------

Create database for Societo before your installation.

(In this section, DBNAME is the name of your new database. And $username or username is a MySQL account)

Log in to MySQL prompt (or access to your phpMyAdmin panel)::

    mysql -u $username -p

Create database to use::

    CREATE DATABASE DBNAME DEFAULT CHARACTER SET utf8;

Grant privilege to your database user (if you need / see also : http://dev.mysql.com/doc/refman/5.6/en/grant.html)::

    GRANT CREAET, DROP, ALTER, INDEX, INSERT, UPDATE, DELETE ON DBNAME.* TO 'username'@'localhost' IDENTIFIED BY 'password';

3. Copy some files and set permissions
--------------------------------------

First, copy the default configuration file. The file in app/config/default/parameters.ini. You need to copy it as app/config/parameters.ini.

And you must set permissions for writing from web server (e.g. change mode to 0777) to the following files:

* app/cache
* app/logs
* app/config/parameters.ini
* web/bundles
* web/image

4. Run the installer
--------------------

Access to the web/index.php from your web browser. Installer will start automatically.

Please input some information in the installer.

5. Remove write permission to configuration file
------------------------------------------------

After install, remove write permission from your app/config/parameters.ini file.

6. Log in to backend and configure
----------------------------------

Access to /admin from your web browser (you may be taked to it by the installer) and log in.

Now, start to create your own social site. Enjoy!

If you want to know about configuration and creation of the site, please visit http://societo.org/documentation/ and read tutorial.
