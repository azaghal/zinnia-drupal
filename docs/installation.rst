Installation
============

Django Conntrackt can be installed through one of the following methods:

* Using *pip*, which is the easiest and recommended way for production websites.


Using pip
---------

In order to install latest stable release of Zinnia Drupal using *pip*, use the
following command::

  pip install zinnia_drupal

In order to install the latest development version of Zinnia Drupal from Github,
use the following command::

  pip install -e git+https://github.com/azaghal/drupal-zinnia#egg=drupal_zinnia

.. warning::

   You will need to update the ``pip`` installation in your virtual environment if you get the following error while running the above command::

     AttributeError: 'NoneType' object has no attribute 'skip_requirements_regex'

   You can update ``pip`` to latest version with::

     pip install -U pip

After this you should proceed to :ref:`configure your Django installation <configuring-django>`.

.. _configuring-django:

Configuring your Django installation
====================================

Once Drupal Zinnia has been installed, you need to perform the following steps
in order to make it available inside of your Django Blog Zinnia project:

#. Edit your project's settings configuration file (``settings.py``), and update
   the ``INSTALLED_APPS`` to include application ``drupal_zinnia``.

After this you will have :ref:`additional management commands available <usage>`
in your Django Blog Zinnia project.
