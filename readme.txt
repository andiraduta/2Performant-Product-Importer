=== 2Performant Product Importer ===
Contributors: 2parale, tetele
Donate link: 
Tags: affiliate, posts
Requires at least: 3.0
Tested up to: 3.0.1
Stable tag: 0.9

Imports products from product feeds in 2Performant affiliate networks.

== Description ==

Use this plugin to insert product data in your posts' custom fields.

It requires authentication as an affiliate in one of these networks. Products are imported as individual posts (or other custom post types, configurable) which can use several custom fields based on product info from the feeds.

Note that you have to embed this information in your theme manually using the `tp_get_the_product_field( $field )` or `tp_the_product_field( $field )` methods. `$field` can be any string defined in the *Product fields* table on the settings page.

== Installation ==

1. Upload `2performant-product-importer` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Configure the plugin's settings
1. Place `<?php tp_the_product_info('info_field'); ?>` in your templates

== Frequently Asked Questions ==

= I have installed the plugin, added a product from a feed, but it doesn't show up on my website. Why? =

You have to manually display the product fields using the `tp_the_product_field( $key )` method.

== Screenshots ==

1. The settings panel

== Changelog ==

= 0.9.1 =
* **New Feature** Introduced ability to insert product info dirrectly into post content using the WYSIWYG editor (see *Insert 2Performant Product* button) and shortcode
* **Bugfix** Product update for drafts/pending products
* **Bugfix** Campaigns now sorted by name 

= 0.9 =
* Initial version.

== Upgrade Notice ==

= 0.9.1 =
Fixes a fatal error shown on environments without required PEAR classes

= 0.9 =
This version is the first version