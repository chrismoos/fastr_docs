Application Settings
=========================

When fastr starts your application, it will read any application-wide settings from the **app/config/settings.rb** file.

Here is an example settings.rb file::

  config.log_level = Logger::DEBUG
  config.cache_templates = false
  
The *config* object allows you to set various settings.