=== PictureBook ===
Contributors: Doc4
Donate link: http://www.doc4design.com/donate
Tags: blogroll, blogroll titles, blogroll images, links, link images, bookmarks, bookmark images
Requires at least: 2.3
Tested up to: 3.5
Stable tag: 1.0



== Description ==

= Plugin URL =
http://www.doc4design.com/plugins/picturebook/

Built for the sole purpose of displaying WordPress bookmark links that show both text and an attached icon. Utilizing the 'Links' tab ( WordPress 2.7 + up ), it is possible to display them as either a list of text links or a list of icon links but not both at the same time.

Enter PictureBook, a small plugin that provides the necessary code to list your bookmarks with both text and icons. An example use might be in the footer of a website that contains social bookmarking links, each link could show the name of the social media website and a small icon next to it just by entering your information into the WordPress' "Links" tab. Achieving this goal is possible with a little core manipulation but we thought it would be more productive to simply install a plugin and not worry about the next WordPress update.

The plugin code itself is just a re-functioning the current wp_list_bookmarks. By altering the link_image output to display the link_name, it becomes possible to achieve our desired effect. The biggest benefit of this plugin is that a user is allowed to display their bookmarks in three separate formats: text-only, image-only and a combination of both.

In the following example, we are using the standard WordPress wp_list_bookmarks formatting with a new function name wp_list_picturebook. All parameters associated with the original tag are functional. The code shown here will display a list of bookmarks with both text and images, no headline and only list those bookmarks from category 4. Because WordPress auto adds our line item tags ( <li> ) they do not need to be included.


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

<code><?php wp_list_bookmarks('title_li=&categorize=0&category=4&show_images=TRUE&show_name=TRUE'); ?></code>
