========
postgres
========

.. note::

    See the full `Salt Formulas installation and usage instructions
    <http://docs.saltstack.com/en/latest/topics/development/conventions/formulas.html>`_.

Available states
================

.. contents::
    :local:

``postgres``
------------

Installs the postgresql package.

``postgres.python``
-------------------

Installs the postgresql python module

``postgres.client``
-------------------

Installs the postgresql client

Testing
=======

Testing is done wit kitchen-salt

``kitchen converge``
--------------------

Runs the postgres main state

``kitchen verify``
------------------

Runs serverspec tests on the actual instance

``kitchen test``
----------------

Builds and runs test from scratch

``kitchen login``
-----------------

Gives you ssh to the vagrant machine for manual testing

Changelog
=========

.. contents::
    :local:

``20150601``
------------

Remove pillar settings to install dev packages. Target postgres.dev at the
minion in the top file to install dev packages.

