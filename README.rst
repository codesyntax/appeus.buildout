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