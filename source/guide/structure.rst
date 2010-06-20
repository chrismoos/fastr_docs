Directory Structure
========================

fastr applications are structured to make your life easy. The structure is very similar to Rails.

* app

  * config
  * controllers
  * models
  * views
  
* custom

  * plugins
  
* public
* lib
* test

app/config
--------------

The config directory contains files for configuring your fastr application.

* init.rb

  * This file is evaluated when your application has finished booting. You can put any initialization code here.

* routes.rb

  * This file is used to configure the routing for your application. See :doc:`routes` for more information.

* settings.rb

  * This file contains settings for configuring fastr. See :doc:`settings` for more information.
  
app/controllers
-------------------

Your controllers should be placed in this directory. See :doc:`controllers` for more information.

app/models
-------------------

Your models should be placed in this directory. Currently there is no persistence in fastr. Use this folder if you want to include a custom persistence module.

app/views
----------------

Your views should be placed in this directory. When a controller renders a template, the template is searched for in this directory. See :doc:`views` for more information.

custom/plugins
-------------------

fastr will load any plugins contained in this directory. See :doc:`plugins` for more information.

public
-------------------

Before routing, fastr will try to serve the file if it exists in this directory. See static files for more information.

lib
--------------------

Put your library code in this directory.

test
---------------------

Put your test files in this directory.

