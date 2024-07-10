=== WP Blame ===
Contributors: lumiblog, wpcornerke
Tags: logs, security, audit, history
Donate link: https://wpcorner.co/donate
Requires at least: 4.0
Tested up to: 6.6
Requires PHP: 5.4
Stable tag: 2.1.6
License: GNU GPL v2
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Keep a record of the activity on your website.

== Description ==

= About =

WP Blame lets you keep a record of everything that has happened on your website by logging the actions of your users in a simple but useful table of data. This plugin is your go-to solution for maintaining a complete audit trail of all user activities on your WordPress site. Whether you're a site administrator, developer, or security professional, WP Blame provides you with the insights you need to keep your site secure and well-managed.

= Key Features =

* **Comprehensive Logging:** Track all user actions including post edits, plugin activations, theme changes, and more.
* **User-Friendly Interface:** View all logged activities in an easy-to-read table right in your WordPress admin area.
* **Detailed Information:** Each log entry includes the user, action type, affected item, and date stamp.
* **User-Based Log Control:** Decide which usernames of people who should not have their actions logged.

= Perfect For =

* Troubleshooting unexpected changes
* Monitoring user activity for security purposes
* Maintaining compliance with audit requirements
* Tracking the history of your site's development and content changes

= Developers =

There are currently no hooks available for this plugin as of yet, however whilst it is discouraged, you can log actions using the `WPB_Log_Hooks::save_new_log` function.

= Stay Updated and Contribute =

WP Blame is an open-source project and we welcome contributions! Follow the development, report issues, or contribute code on our [GitHub repository](https://github.com/wpcorner/wp-blame).

= Privacy Notice =

WP Blame logs user activities on your WordPress site. This includes usernames, IP addresses, and details of actions performed. Please ensure you have necessary consent and include this information in your site's privacy policy if required by local laws and regulations.


== Screenshots ==

1. An example of the logs table.
2. The Settings page

== Installation ==

1. Upload the `wp-blame` folder to the /wp-content/plugins/ directory
2. Activate the plugin through the `Plugins` menu in WordPress
3. Configure the plugin settings under `Settings > WP Blame`

== Frequently Asked Questions ==

= What kind of things will be logged? =

Almost anything that can be logged, is logged. This includes but is not limited to posts, terms, media and users as well as general options.

= Can I log a custom action by another plugin? =

You can, but it's not advised as the Log API has not bee fully developed yet and may not work very well with other plugins. `WPB_Log_Hooks` is the class that handles logging.

= Can I only log particular users? =

You can add usernames to a whitelist of people who's actions should not be logged on the website.

= Is WP Blame compatible with multisite installations? =

Yes, WP Blame is fully compatible with WordPress multisite installations.

== Changelog ==

= 2.1.6= 

* Fixed critical error causing "Division by zero" in log list pagination 
* Improved overall plugin stability and security 
* Enhanced compatibility with latest WordPress version

= 2.1.5 = 

* Updated plugin author information 

= 2.1.4 = 

* Updated author information 

= 2.1.3 = 

* Updated author information - Removed Daniel James danieltj

= 2.1.2 =

* Updated for new developer to maintain.

= 2.1.1 =

* Updated the plugin translations to be in en_US by default.
* Fixed a bug relating to terms being shown in the log table.
* Minor improvements to some translation strings.
* Minor updates to the plugin readme.txt file.

= 2.1 =

* Fixed a bug where the per page option wasn't added on install.
* Fixed a bug with the item column being blank after deletion.
* Fixed an untranslated string for the logs per page option.
* Minor improvements to a variety of core functions.

= 2.0 =

* Major rewrite of the entire plugin code.
* Changed the license from GNU GPL v2 to v3.

== Upgrade Notice ==

= 2.1.6 = 

* Major Fix: Fixed the error occurring in the 'prepare_items()' method, specifically in the pagination calculation..
