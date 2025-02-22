=== WP-Hashcash Extended  ===
Contributors: azizmb, ecb29, donncha
Tags: spam, antispam, anti-spam, comments, comment, pingback, trackback, wp-hashcash, plugin, security, wordpress, javascript, js, signup, sign-up, wp-login.php, wp-signup.php, buddypress, bp, WPMU
Tested up to: 3.3.1
Stable tag: 4.7
Requires at least: 3.1

Client-side javascript blocks all spam bots. XHTML 1.1 compliant. Now with support for WordPress Versions 3.1+

== Description ==

= No More Spam =

WP Hashcash is an antispam plugin that eradicates comment spam on Wordpress blogs. It works because your visitors must use obfuscated javascript to submit a proof-of-work that indicates they opened your website in a web browser, not a robot. If the javascript check fails, WP Hashcash now gives you three options; it can either put the comment into moderation (default), put the comment in the akismet queue, or delete it.

You can read more at the [WP Hashcash plugin](http://azizmb.com/2012/04/wp-hashcash-now-working-on-newer-wordpress-versions/) page.  WP Hashcash is 100% GPL compatible.

= Features =

1. Blocks all comment spam, but not real comments
2. Also prevents most trackback / pingback spam
3. Also protects signup pages for Wordpress (WP), BuddyPress (BP), and Wordpress Multi-User (WPMU)
4. Widget support to display spam statistics and edit the configuration
5. Works with IE, Firefox, and Safari
6. 100% standards compliant XHTML 1.1, works with jQuery and Prototype
7. Tested with Wordpress 3, Firefox, Safari, IE, and Chrome
8. Akismet compatibility

= Limitations =

WP Hashcash relies on the presence of two hooks in your theme, `wp_head` and `comment_form`. If your theme doesn't include these actions, you will need to add them immediately before the end head and end form tags respectively.

== Installation ==

= Installation Instructions =

To install WP Hashcash, please download the plugin and unzip it, then copy the wp-hashcash.php file to wp-content/plugins. Activate the plugin and drag into your Widgetized sidebar for public statistics, or visit Options, WP Hashcash from the admin panel to configure options.

= Notes =

If you are upgrading from a previous version of WP-Hashcash, please disabled the plugin, then delete its files entirely.  Then, upload the latest plugin files and activate!

== Screenshots ==

1. Wordpress Hashcash Options Screen

== Testimonials ==

* "One of my favorites"
* "this is a clever idea that I think might work well"
* "I haven't had a single comment spam in my comment moderation queue for over a week now. I'm feeling the love!"
* "The least annoying one I have found"
* "this thing was a trivial install"
* "a fancier technique"
* "Comment Spam is a thing of the past, and I owe it to Spam Stopgap Extreme. If you use WordPress, I highly recommend installing this plugin. It has completely eliminated the comment spam problem I was having. I no longer need the spammer Tarpit plugin, or anything."
* "Why am I not worried about comment spam anymore? Because of my awesome new blog plugin, Spam Stopgap Extreme. This baby blocks any bot trying to post to my blog. No blacklists, no moderation, no 'spam points', no nothing. You won't even know that it's working."
* "I haven't had anything to 'deal' with in several weeks. That's a nice thing. I've also had a bunch of folks leave legitimate comments that have gotten through. It's all good."

== Upgrade Notice ==

= 4.7 =
Fixed capability for WordPress 3.1+

== Changelog ==
= 4.7 =
* Fixed capability for WordPress 3.1+

= 4.6 =
* Removed links from the blog linking back to Hashcash homepage to comply with WordPress.org plugin guidelines. Props Ryan Hellyer.

= 4.5.1 =
* Fix a javascript error

= 4.5 =
* Support clean interoperation with jQuery and Prototype
* Protect BuddyPress (BP) signup pages

= 4.4 =
* Admin users can now comment from Dashboard
* Tested on WP 2.9.2 in Chrome, IE, and FF
* Fix a potential JS error

= 4.1 =
* Added a new options page under Options, Wordpress Hashcash
* Fixed XHTML standards compliance
* Added validation options for pingbacks and trackbacks (stolen from here)
* Added a logging option for moderated comments

= 4.0.5 =
* Added an option for handling comments via moderation, the akismet queue, or deletion
* Removed database dependencies
* Removed error message for hash fail
* Added the noscript tag for users without javascript
* Corrected the widget formatting
* Changed zip file format from winrar to 7zip, hopefully it will be more compatible

= 4.0.4 =
* Removed version checking
* Removed an unnecessary link element in the head section

= 4.0.3 =
* Suppress errors on loading remote version by any method
* Fix typo-bugs everywhere affecting the widget reporting, date checking, etc
* Strip tags from remote version
* Try various methods to get remote version, ignore if we can't open sockets
* Fix a bug with one of the javascripts
