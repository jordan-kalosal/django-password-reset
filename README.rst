Django-password-reset-mandrill
=====================
Forked from https://travis-ci.org/brutasse/django-password-reset.
This fork empowers django-password-reset to use Mandrill to send emails.  
It is assumed that https://github.com/brack3t/Djrill (Djrill) is installed to replace
standard Django email functionality with Mandrill transactional emails.

All instructions and features of django-password-reset still apply.


.. image:: https://travis-ci.org/brutasse/django-password-reset.svg?branch=master
   :alt: Build Status
   :target: https://travis-ci.org/brutasse/django-password-reset

Class-based views for password reset, the usual "forget password?" workflow:

* User fills his email address or username
* Django sends him an email with a token to reset his password
* User chooses a new password

The token is not stored server-side, it is generated using Django's signing
functionality.

* Author: Bruno Renié and `contributors`_
* Licence: BSD
* Compatibility: Django 1.4+ (cryptographic signing needed)

.. _contributors: https://github.com/brutasse/django-password-reset/contributors

Installation
------------

* Download this repository, copy the ``password_reset`` folder to your project directory (same level as manage.py)
* Add ``password_reset`` to your ``INSTALLED_APPS``
* Include ``password_reset.urls`` in your root ``urls.py``

For extensive documentation see the ``docs`` folder or `read it on
readthedocs`_

.. _read it on readthedocs: http://django-password-reset.readthedocs.org/

