======================================
Command Line Installation (Incomplete)
======================================

You may feel pain by web installer because you are good at using CLI interfaces.

Societo also prepares the way of installation from command line. This document explain it for you.

Requirements
============

Please read "Requirements and Optionals" section of :doc:`standard`.

You can check your system configurations by executing app/check.php script::

    $ php app/check.php

Installation
============

1. Download and extract Societo package
---------------------------------------

Please read "Download and extract Societo package" section of :doc:`standard`.

2. Create database (you may skip this section if you already have)
------------------------------------------------------------------

Please read "Create database" section of :doc:`standard`.

3. Copy some files and set permissions
--------------------------------------

Please read "Copy some files and set permissions" section of :doc:`standard`.

But, you don't need to set write permission from web server to the following:

* app/config/parameters.ini
* web/bundles

4. Write configuration file
---------------------------

Edit app/config/parameters.ini for your needs. The followings are description about configuration items.

database_driver (mandatory)
    Database driver name which Doctrine can regognize. `pdo_mysql` is official supported driver.

secret (mandatory)
    Societo uses this value in many situations for keeping security of the site. DON'T CHANGE THIS VALUE AFTER THE INSTALLATION!
    And you specify the same value in the barancing web server.

5. Cache clear
--------------

Clear cache because change your configuration::

    $ php app/console cache:clear

6. Install assets
-----------------

Install assets file::

    $ php app/console assets:install --symlink web/

7. Create database
------------------

Create database::

    $ php app/console doctrine:schema:create --dump-sql > /path/to/sql
    $ mysql -u root --default-character-set=utf8 DBNAME < /path/to/sql


