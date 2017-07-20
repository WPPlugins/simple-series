=== Plugin Name ===
Contributors: MakerBlock
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=EYYL4BEFYRJF2
Tags: series, simple series, series of posts, posts series, post organization, organize series, series organization, post, posts, shortcode, short code, organize, issues, magazine, article, articles, list, organization, series organization
Requires at least: 3.3
Tested up to: 3.5.1
Stable tag: 1.4.6

An easy to use shortcode for automatically creating and organizing a series list for multiple posts on the same topic with appropriate SEO attributes.

== Description ==

Simple Post Series with SEO! uses a WordPress shortcode to associate your posts together, with a little extra SEO mojo for good measure.  All you have to do is use the shortcode in each of the posts you want in the same series and the plugin does the rest.  It automatically finds all of the posts with the same shortcode, organizes them by publication date, and presents them in a professional and easy to read format with appropriate SEO tags.  If you wish to change the formating, you can just add your own custom CSS to your theme.  

I've now added a button to the TinyMCE text editor that will allow you to select a series shortcode from the list of titles you've already used.  (Don't worry!  I'm working on a button for the visual editor...)

If you like this plugin, <a href="http://wordpress.org/extend/plugins/simple-series/">please give it a 5-star rating over here --></a>

This simple series plugin doesn't clutter up your WordPress installation with unnecessary settings.  It doesn't create extra tables, content types, or taxonomies.  It doesn't require a special version of WordPress or the very latest features of PHP or MySQL.  Neither are there any unnecessary options, buttons, settings to mess with.

And, you can always <a href="http://makerblock.com/2012/01/simple-series-wordpress-plugin/">visit my website</a> (It's mostly about awesome open source robots, if you're into that kinda thing).

== Installation ==

This section describes how to install the plugin and get it working.

1. Upload `simpleseries.php` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Decide on the title for your series of posts
1. Add the following shortcode to each post in your series `[simple_series title="This Is My Series Title"]`  Or, if you're using the TinyMCE text editor, you can click the button "Add Series" to choose from a series title you've already used or create a new series.
1. Now every post with that exact same shortcode will automatically have a neatly organized list of all posts in the series, in chronological order!

== Frequently Asked Questions ==

= How does "Simple Post Series with SEO!" work? = 

Easy!  Just add the shortcode to each of the posts you want to put in the series.  Inside the shortcode you will need to specify the title for the series. Like so:<br> `[simple_series title="This Is My Series Title"]`

= What if I add more posts later? =

No problem!  The "Simple Post Series with SEO!" plugin will always update the series lists in each of your posts whenever you publish a new post.  The newest post will always be added to the series in chronological order, by publication date.  You can see an example of what it looks like here in my own DrawBot series.

= What if I add one post to multiple series? =

No problem!  Just include a comma between the series titles in the shortcode.  It will add your post to each series named and it will display each associatd series list.
<ul>
<li> Example of just a post in only one series `[simple_series title="This Is My Series Title"]`</li>
<li> Example of just a post in two series `[simple_series title="This Is My Series Title,This Is A Totally Different Series Title!"]`</li>
</ul>

= It's a piece of crap!  It doesn't work! = 

Calm down - everything will be okay.  If you've activated the plugin, added the shortcode with a title, and updated/published your post, and you don't see the series list, try to refresh the page in your browser or clear the page cache.

= Hey!  This formatting sucks!  Can I add my own CSS? =

Sure!  There are three components to the series list: the DIV wrapper, the title of the series inside SPAN tags, and the list items.  This is the exact formatting I use in my blog.  If you need something different, just fiddle with the CSS to suit and add them to your stylesheet.
<br> `div.mbk_simple_series_wrapper { display:block; }`
<br> `span.mbk_simple_series_title { font-weight:bold; display:block;}`
<br> `div.mbk_simple_series_wrapper ol li.mbk_simple_series_list_item, a.mbk_simple_series_link_prev, a.mbk_simple_series_link_next { font-size:smaller; line-height: 0.8em;}`
<br> `a.mbk_simple_series_list_current_item { font-weight:bold;}`
<br> `a.mbk_simple_series_link_prev { float:left; }`
<br> `a.mbk_simple_series_link_next { float:right; }`

= Wait!  I have more questions! = 

Please <a href="http://makerblock.com/2012/01/simple-series-wordpress-plugin/">visit my website</a> or <a href="http://makerblock.com/contact/">send me an e-mail!</a>

== Screenshots ==

1. An example of the shortcode as it appears in the post editor
2. The same shortcode from the same post, as it appears to someone reading the post
3. The same shortcode from the same post, with CSS formatting as suggested in the FAQ

== Changelog ==

= 1.4.6 = 
* 3/2/2013: Now the plugin works with posts, pages, or a combination of posts and pages.  I've also added a button to the TinyMCE text editor so you can add an existing or new series title with just a few clicks.

= 1.4.5 = 
* 2/6/2012: Now the plugin adds a class to the link to the current post in the series.  This makes it easy for you to highlight this link with CSS, if you wish.  I've added the example CSS to the FAQ.  This makes it a little easier for the reader to find where the post is in the series.  Thanks to insomnia for the inspiration!

= 1.4.4 = 
* 2/4/2012: Now the plugin supports adding a post to multiple series!  Thanks to Dale for the suggestion!

= 1.4.3 = 
* 2/3/2012: Added an FAQ item suggesting users refresh thier page if they don't see the list after publishing.

= 1.4.2 = 
* 1/31/2012: A new screenshot showcasing the series appearance with CSS formatting

= 1.4.1 = 
* 1/27/2012: Better information about CSS formatting, with examples

= 1.4 = 
* 1/27/2012: FAQ gives some guidance on how to style the series lists.  
* 1/27/2012: A very slight change to the series list formatting.  (I changed the list title from having a class to having an id tag).

= 1.3 = 
* 1/27/2012: Simplifying the plugin a little, adding a "to do" list

= 1.2 =
* 1/26/2012: Now the series shows up properly in RSS feeds too!

= 1.1 =
* 1/26/2012: Now the plugin supports multiple separate post series!

= 1.0 =
* Initial release on 1/25/2012!

== To Do List ==
* Create an uninstall button - it would delete ALL post meta info that was associated with a key of "mbk_simple_series"
* Create a way to rename an entire series.  This would take a fair bit of work - since the shortcode inside each post would have to be edited.  It's not that easy, but totally doable.
* Consider storing all simple_series lists in a single plugin option, rather than in the post meta.  This would actually help with speed/efficiency since it would cache the results.  This would also make it slightly easier to uninstall.
* Consider reducing the number of posts listed in a series list.  It could be hidden/revealed via jQuery.