=== PictureBook ===
Contributors: Doc4
Donate link: http://www.doc4design.com/donate
Tags: blogroll, blogroll titles, blogroll images, links, link images, bookmarks, bookmark images
Requires at least: 2.3
Tested up to: 2.9.1
Stable tag: 1.0



== Description ==

"PictureBook" allows for the combination of both text and images when displaying a list of bookmarks. As with the case of this web site the footer contains a few social bookmarking links each containing the name of the social bookmarking site and a small icon all through the wonderful world of WordPress’ “Links” tab.

Achieving this goal is possible with a little core manipulation but we thought it would be more productive to simply install a plugin and not worry about the next WordPress update. The plugin code itself is a simple matter of re-functioning the current wp_list_bookmarks. By altering the link_image output to display the link_name it is possible to achieve the desired effect. The biggest benefit of this plugin is that a user is allowed to display their bookmarks in three separate formats: text-only, image-only and now a combination of both.


== Screenshots ==

View Screenshots:
http://www.doc4design.com/plugins/picturebook


== Installation ==

To install the plugin just follow these simple steps:

1. Download the plugin and expand it.
2. Copy the picturebook folder into your plugins folder ( wp-content/plugins ).
3. Log-in to the WordPress administration panel and visit the Plugins page.
4. Locate the PictureBook plugin and click on the activate link.
5. Replace wp_list_bookmarks with wp_list_picturebook



== Frequently Asked Questions ==

= Can't I do this with WordPress? =

With more recent versions of WordPress using the following code will achieve the same effect by way of "show_images=TRUE&show_name=TRUE": 

<?php wp_list_bookmarks('title_li=&categorize=0&category=4&show_images=TRUE&show_name=TRUE'); ?>
