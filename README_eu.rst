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