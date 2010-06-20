Getting Started
============================

Install
------------------

There are two ways to install fastr. You can install the latest version from rubygems, or install from the latest git source.

Rubygem
^^^^^^^^^^

.. code-block:: bash

  $ sudo gem install fastr

Source
^^^^^^^^^^

.. code-block:: bash

  $ git clone git://github.com/chrismoos/fastr.git
  $ cd fastr
  $ sudo rake install
  
  
Initialize
--------------------------

To setup a fastr application, you can use the fastr command.

.. code-block:: bash

  $ fastr init helloworld
  
Starting
----------------------------

To start your fastr application using thin, issue the following command:

.. code-block:: bash

  $ thin -p 5000 start

You should see the following output:

.. code-block:: bash

  >> Using rack adapter
  >> Thin web server (v1.2.7 codename No Hup)
  >> Maximum connections set to 1024
  >> Listening on 0.0.0.0:5000, CTRL+C to stop
  [INFO] [Fastr::Application]: Loading application...
  [DEBUG] [Fastr::Plugin]: Loading plugins...
  [DEBUG] [Fastr::Application]: Loading lib classes...
  [DEBUG] [Fastr::Application]: Loading model classes...
  [DEBUG] [Fastr::Application]: Loading controller classes...
  [DEBUG] [Fastr::Router]: Loading routes from: /private/tmp/helloworld/app/config/routes.rb
  [DEBUG] [Fastr::Router]: Adding route, path: /:controller/:action, args: []
  [INFO] [Fastr::Application]: Application loaded successfully.
  
Try to access your application by going to the URL:

`http://localhost:5000 <http://localhost:5000>`_