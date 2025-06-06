=== Action Network ===
Contributors: concertedaction
Tags: signup, events, action network, online organizing
Requires at least: 4.6
Tested up to: 6.5.2
Stable tag: 1.4.4
License: GPLv3 or later
License URI: https://www.gnu.org/licenses/gpl.html

Provides Action Network (actionnetwork.org) action embed codes as shortcodes and a calendar and signup widget

== Description ==

A free Wordpress plugin for the [Action Network](https://actionnetwork.org) online organizing tools maintained by [Concerted Action](http://concertedaction.consulting/).

Features:

* Create a Wordpress shortcode or widget from any Action Network embed code.
* Manage your saved embed codes using the Wordpress backend. Supports sorting by title, type and last modified date, and provides a search function.
* Modify Action Network's default "thank you for your support" and "help us by using sharing tools" messages, and control which sharing options (social, email & embed codes) are displayed, using shortcode options or widget controls.
* Use `[actionnetwork_list]` shortcode or Action Network List widget to show a list of current actions.
* Use `[actionnetwork_calendar]` shortcode or Action Network Calendar widget to show a list of upcoming events. Optionally outputs upcoming events in JSON. Development of this feature was supported by [The People's Lobby](http://www.thepeopleslobbyusa.org/) - if you like it, please consider [making a donation to them](https://actionnetwork.org/fundraising/donate-to-the-peoples-lobby).
* If you are an [Action Network Partner](https://actionnetwork.org/partnerships), use your API key to sync all of your actions from Action Network to Wordpress.
* Create signup widgets which allow visitors to your site to sign up for your email list _without_ using Action Network javascript embeds. This allows you to place a signup form on every page (for example in the sidebar), and still load Action Network embed codes for actions on particular pages (since Action Network's scripts will only load one embed code per page).  This feature does require the API key, so you have to be an [Action Network Partner](https://actionnetwork.org/partnerships) to use it.

Detailed specs for shortcode attributes, widget options, etc. are available on the Help menu for the Action Network page on the backend.

== Installation ==

1. Upload the plugin files to the `/wp-content/plugins/plugin-name` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress
1. If you have an [Action Network API Key](https://actionnetwork.org/partnerships), go to the Action Network section and click on the "Settings" tab to enter your API key. Your actions will automatically be synced from Action Network to your Wordpress site.

== Frequently Asked Questions ==

= My ticketed events aren't showing up on the list =

Action Network does not currently provide access to Ticketed Events through its API. You can, however, use the "Add Action" tab and copy and paste the embed code manually.

== Screenshots ==

1. Provides a Wordpress-like interface for managing embed codes and shortcodes

== Changelog ==

= 1.4.4 =

* Security updates. 
* Updated and tested with latest Wordpress version.

= 1.4.3 =

* Security updates. 
* Updated and tested with latest Wordpress version.

= 1.4.2 =

* Bug fix for to support embedded Action Network URLs up to version 4.

= 1.4.1 =

* Bug fix for widget hCaptcha protection when hCaptcha keys are not provided. The hCaptcha verification will require both hCaptcha keys in the plugin settings and the "Spam protection" checkbox be enabled. If either are not provided, hCaptcha protection will be disabled, allowing the form to be submitted without verification.

= 1.4.0 =

* Fixed hCaptcha checkbox.

= 1.3.0 =

* Updated automatic syncing of data from Action Network. 
* Added record of sync results.

= 1.2.2 =

* Revert of SVN issue.

= 1.2.1 =

* Added Gutenberg Editor button.
* Bug fix related to hCaptcha.

= 1.2 =

* This major update includes the following updates: 
* hCaptcha ability added for API based forms. 
* Bug fixes related too multiple embeds on a single page, and the API sync. 
* shortcode button for tinymce WYSIWYG. 
* additional documentation on setting page. 

= 1.1.3 =

* Updating developer information.

= 1.1.2 =
* Fixed problem where Action Network dates (both for events and modified_date for all actions), which are in local time, were being compared to UTC time. Now they are compared to the local timezone of the website.

= 1.1.1 =
* Fixed problem which would cause updates from wordpress.org to crash

= 1.1.0 =
* Added AJAX submission for signup form, new shortcode attributes to control thank-you displays, new widget to display actions, and new shortcode and widget to display lists of actions.

= 1.0.1 =
* Updated to recognize Action Network's v3 widgets

= 1.0 =
* First release on wordpress.org

Previous development versions can be found on [github](https://github.com/jkissam/actionnetwork/)

== Upgrade Notice ==

= 1.2.1 =

Added Gutenberg Editor button.

= 1.2 =

This major update includes the following updates: 
hCaptcha ability added for API based forms. 
shortcode button for tinymce WYSIWYG. 

= 1.1.1 =
Fixed problem which would cause updates from wordpress.org to crash

= 1.1.0 =
New features, including new widgets, shortcodes, and shortcode options, as well as ajax submission of the signup form.

= 1.0.1 =
Updated to recognize Action Network's v3 widgets

= 1.0 =
Install from wordpress.org to stay up-to-date
