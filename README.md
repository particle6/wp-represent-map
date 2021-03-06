WP REPRESENT MAP
================

Wordpress plugin based on [Represent Map][1].

The original represent map is a full-system to manage startups, accelerators, coworking and much more pin on maps using Google Maps API.

This plugin is inspired on the original Represent Map providing 
the wordpress admin management. The same functionality inside Wordpress.


INSTALLATION
==========

Composer
--------

    "andrebian/wp-represent-map": "dev-master"

Cloning
------
 Clone this repository into your wp-content/plugins path keeeping the wp-represent-map path name and enable it on Wordpress admin panel.
 
Downloading as zip
-----------------

Download it as zip, unzip into your wp-content/plugins path keeping the wp-represent-map path name.

USAGE
======

Indispensable
--------------
On your functions.php put the following code:

    /* Single item height in pixels */
    if ( !defined('SINGLE_HEIGHT_MAP') ) {
        define('SINGLE_HEIGHT_MAP', '150PX');
    }

    /* Full map height in pixels */
    if ( !defined('ALL_HEIGHT_MAP') ) {
        define('ALL_HEIGHT_MAP', '560px');
    }

After this follow the steps bellow.

Admin Panel
----------
Configure your default location and default lat lng in **Settings/Wp Represent** Map admin page. After this create your item types in **Map Items/Type** on wordpress admin panel. Now just create your Map items providing the correct address and selecting which is the type of it.

Blog/Site
---------

The WP Represent Map works with shortcode. To show all items in a map use:

    [represent-map]
    
    
To show only one type of items on map provide the slug you want to show in **type** parameter:

    [represent-map type=startup]


NOTE
=============

This plugin actually works with only 2 category levels, if exists more than 2 levels 
the following WILL NOT APPEAR on lateral menu.

    

CONTRIBUTING
=============

I am just starting the development and would be very happy if anyone 
can help to create an awesome tool.

If you want to contribute, please read [CONTRIBUTING][2] file.


  [1]: https://github.com/abenzer/represent-map
  [2]: https://github.com/andrebian/wp-represent-map/blob/master/CONTRIBUTING.md