Description
-----------
This module provides a method for Migrating drupal from an existing version to another.


Installation
------------
To install this module, do the following:

1. Extract the tar ball that you downloaded from Drupal.org.

2. Upload the entire directory and all its contents to your modules directory.

3. Edit your settings.php file to recognize the 2 databases you will be importing from.

For example:

$databases = array (
  'default' => //Our New db
  array (
    'default' => 
    array (
      'database' => 'viapp_d7',
      'username' => 'user',
      'password' => 'password',
      'host' => 'localhost',
      'port' => '',
      'driver' => 'mysql',
      'prefix' => '',
    ),
    ),
  'legacy' => //We can call this legacy
  array (
  'default' => 
    array (
      'database' => 'viapp_d5',
      'username' => 'user',
      'password' => 'password',
      'host' => 'localhost',
      'port' => '',
      'driver' => 'mysql',
      'prefix' => '',
    ),
  ),
);

Configuration
-------------
To enable and configure this module do the following:

1. Go to Admin -> Modules, and enable Viapp_Import.

2. Go to Admin -> Content -> Viapp Import.