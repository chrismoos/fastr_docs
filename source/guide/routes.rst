Routes
===========

fastr searches your routes to determine which controller and action a path belongs to.

Routes are configured in the **app/config/routes.rb** file. Here is an example::

  router.draw do |route|
    route.for '/:controller/:action'
    route.for '/home/:action', :action => '[A-Za-z]+'
    route.for '/test', :to => 'home#index'
  end
  
Variables
-------------

Inside of your route you can use variables. These variables will be available in your controller's *params* object. By default variables are matched with the regex **\w+**. You can override this by specifying the variable name and the regex to use.

Example::

  route.for '/view/post/:id', :id => '[0-9]+'
  

If the URL was **/view/post/1**, the *params* object in the controller would look like this::

  {:action=>"index", :id=>"1", :controller=>"main"}