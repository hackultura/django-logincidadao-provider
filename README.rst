=============================
Django Login Cidadão Provider
=============================

.. image:: https://badge.fury.io/py/django-logincidadao-provider.png
    :target: https://badge.fury.io/py/django-logincidadao-provider

.. image:: https://travis-ci.org/hackultura/django-logincidadao-provider.png?branch=master
    :target: https://travis-ci.org/hackultura/django-logincidadao-provider

Provider do Login Cidadão para projetos Python. Esse provider será independente, e que pode ser inserido nos projetos
em Django. Ele foi construido em base do [django-allauth](https://github.com/pennersr/django-allauth).

Documentação
-------------

Toda a documentação está em https://django-logincidadao-provider.readthedocs.org.

Instalação
----------

1. Instale a dependência:

.. code-block:: bash

    $ pip install django-logincidadao-provider

2. Registre a aplicação em ``INSTALLED_APPS``:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'django.contrib.sites',

        'allauth',
        'allauth.account',
        'allauth.socialaccount',
        'logincidadao_provider',
    )

3. Defina o seu ``CLIENT_ID`` e o ``SECRET_KEY`` no seu ``settings.py``:


.. code-block:: python

    LOGINCIDADAO_DOMAIN = 'http://meu.logincidadao.org.br/'
    LOGINCIDADAO_PUBLIC_KEY = 'asl1209aslk'
    LOGINCIDADAO_PRIVATE_KEY = 'ak(!@akase1!@(asjaslk9110'

 Licença: GPLv2
