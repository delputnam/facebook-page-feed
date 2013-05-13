=== FBF Facebook page Feed Widget ===
Contributors: lakshmananphp
Donate link: http://lakshmania.wordpress.com/
Tags: facebook, facebook sidebar, sidebar, social sidebar, widget, plugin, posts, links, facebook widget, facebook page,facebook page feed,facebook feed
Requires at least: 3.3+
Tested up to: 3.5.1
Stable tag: 1.2.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Shows the latest updates from one or multiple Facebook page(s) in a sidebar widget with short code feature.

== Description ==
This plugin displays the latest posts from one or multiple Facebook page(s) in a sidebar widget. 
Facebook page ID is enough to configure this widget.

This plugin uses simplepie rss reader which is a in-built/default reader for wordpress.

Bug fixes / changes in this version:
* wordpress HTTP header error message will be shown in case of any errors.
* Feed are not cached now. So feeds will update on page refresh.
* Update time is corrected.
* Added option to show/hide facebook like button inside the feed.
* ul li issued fixed. the plugin outputs standard html now
* css changes - container bg color and width removed. (If you use shortcode inside a post/page, the feed will occupy whole content content area)


= Note =
* FBF Facebook page Feed Widget requires PHP5
* You can display the feeds which are publicly accessible
* Provide multiple pages id sepearated by commas e.g id1,id2,id3,id4

== Installation ==
1. Upload the `FBF Facebook page Feed Widget` directory into the `/wp-content/plugins/` directory
2. Activate the plugin through the `Plugins` menu in WordPress
3. Inside the `Themes->Widget` menu, place the FBF Facebook page Feed Widget inside a sidebar, customize the settings and save
4. Enter facebook page id(s)
5. Enjoy!

Multiple Page Feed

* Provide multiple pages id sepearated by commas
e.g id1,id2,id3,id4


Short code

[fbf_page_feed pageID="133662330114199" num="2" show_description="true" update="true" show_avatar="true" avatar_size="square" link_target_blank="true" feed_title = "true" like_button="true" like_button_position="top"]

* update="true" = shows timestamp
* avatar_size="square" = avatar size, you can choose square,small,large and normal
* feed_title = "true" to show feed title
* feed_title = "" to hide feed title
* like_button = "true" to show facebook like button
* like_button_position = "top" to show facebook like button after every feed title
* like_button_position = "bottom" to show facebook like button after every feed description

To display feeds in Template (page templates - in themes)

You can use the following code to to display Facebook page feed in any part of template

do_shortcode('[fbf_page_feed pageID="133662330114199" num="2" show_description="true" update="true" show_avatar="true" avatar_size="square" link_target_blank="true" feed_title = "true" like_button="true" like_button_position="top"]');
we are using shortcode function to render the widget
do_shortcode will convert that shortcode to output, and we echo the output.


== Frequently Asked Questions == 

= I dont know my facebook page ID, How can i find it? =

To find your Page ID, simply go to your "Facebook Page", Click "Edit Page" button.
Then go to your browser address bar and copy your Page ID. (example:http://www.facebook.com/pages/edit/id?XXXXXXXXXX)
Your Id will be the number next to question mark.

== Credits ==

http://wordpress.org/support/profile/lakshmananphp


== Screenshots ==
1. Configuring widget in admin panel  
2. Example feed in front end sidebar
3. Example feed in front end within content of a post (using shortcode)
4. 2 different feeds (mashable fb page feed in content area & FBF widget feed in sidebar) 
== Changelog ==
= 1.2.1 =
* wordpress HTTP header error message will be shown in case of any errors.
* Feed are not cached now. So feeds will update on page refresh.
* Update time is corrected.
* Added option to show/hide facebook like button inside the feed.
* ul li issued fixed. the plugin outputs standard html now
* css changes - container bg color and width removed. (If you use shortcode inside a post/page, the feed will occupy whole content content area)

= 1.2 =

* simplexml_load_file() issues fixed.
* Added option to show multiple page feed.
* Broken links in feed description fixed
* Added option to show/hide facebook feed title.

= 1.1 =

* Added option to show/hide facebook avatar.
* Added stylesheet with simple predefined styles.
* Shortcode feature added to support facebook page feed widget in post/page content.

= 1.0 =
* Initial version


== Upcoming features ==

* showing feeds with jquery cycle
* predefined themes for widget

 == Upgrade Notice ==
* version 1.2.1 - feeds will update regularly, no caching now. posted time is corrected, you can add like buttons for every item in feed
* version 1.2 - simplexml_load_file() issues fixed, Added option to show multiple page feed, Broken links in feed description fixed
* version 1.1 - Added option to show/hide facebook avatar.
