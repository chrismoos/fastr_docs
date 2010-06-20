.. Fastr documentation master file, created by
   sphinx-quickstart on Sun Jun 20 15:49:24 2010.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

fastr
=================================

fastr is an event-based web framework for Ruby.

Quick Start
----------------

You can setup a fastr application by doing the following.

.. code-block:: bash

  $ sudo gem install fastr
  $ fastr init helloworld
  $ cd helloworld
  $ thin -p 5000 start

Guide
--------------------

.. toctree::
   :maxdepth: 1
   
   guide/setup
   guide/structure
   guide/settings
   guide/routes
   guide/controllers
   guide/views
   guide/plugins

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

