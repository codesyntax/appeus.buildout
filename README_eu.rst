================
appeus webgunea
================

Webgunea martxan jartzeko egin beharreko pausuak:

Zerbitzaria konpilatu::

    $ virtualenv-2.7 .
    $ ./bin/python bootstrap.py
    $ ./bin/buildout -c deployment.cfg -vv


Zerbitzuak martxan jartzeko::

    $ ./bin/supervisord

Zerbitzuak gelditzeko::

    $ ./bin/supervisorctl shutdown


Apache eta Nginx web zerbitzarietan erabili daitekeen konfigurazioa `etc` karpetan izango duzu, egin fitxategi horren esteka bat zure zerbitzariaren konfigurazio-fitxategiak dauden karpetara.

Dependentziak
==============

Debian/Unbuntu erako zerbitzarietan::

    $ sudo apt-get install build-essential subversion-tools git git-core libxslt1-dev libxml2-dev libjpeg8 libjpeg8-dev libfreetype6 libfreetype6-dev libssl-dev python-setuptools python-virtualenv unzip libzip-dev libzzip-dev libzzip-0-13 zlib1g-dev zlib1g libtar0 libtar-dev liblz1 liblz-dev libbz2-dev python2.7 python2.7-dev


Eguneratu sistemako virtualenv eta setuptools::

    $ sudo pip install --upgrade virtualenv setuptools

Webgune honek python-en 2.7 bertsioarekin funtzionatzen du. 2.6 bertsioarekin ere funtzionatu dezake baina ez dugu probatu. Ez du python 3 edo python 2.5 edo lehenagokoekin funtzionatzen.