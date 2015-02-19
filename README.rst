===============
appeus website
===============

To have this site running:

First, compile everything::

    $ virtualenv-2.7 .
    $ ./bin/python bootstrap.py
    $ ./bin/buildout -c deployment.cfg -vv


Then start the services::

    $ ./bin/supervisord

To stop the services::

    $ ./bin/supervisorctl shutdown


A configuration file for Apache and Nginx will be created inside `etc`, just symlink into the configuration folder of your server.

Dependencies
==============

Debian/Unbuntu servers::

    $ sudo apt-get install build-essential subversion-tools git git-core libxslt1-dev libxml2-dev libjpeg8 libjpeg8-dev libfreetype6 libfreetype6-dev libssl-dev python-setuptools python-virtualenv unzip libzip-dev libzzip-dev libzzip-0-13 zlib1g-dev zlib1g libtar0 libtar-dev liblz1 liblz-dev libbz2-dev python2.7 python2.7-dev


Upgrade virtualenv and setuptools::

    $ sudo pip install --upgrade virtualenv setuptools

This website works with python 2.7. It could work with python 2.6 but we haven't tested it. It will not work with python 3 or python 2.5 or previous.