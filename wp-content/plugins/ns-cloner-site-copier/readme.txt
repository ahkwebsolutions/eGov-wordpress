=== NS Cloner - Site Copier ===
Contributors: neversettle
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=53JXD4ENC8MM2&rm=2
Tags: automate, duplicate, copy, copy site, copier, clone, clone site, cloner, multisite, network, subdomain, subdirectory, subfolder, template
Requires at least: 3.0.1
Tested up to: 5.2.1
Requires PHP: 5.6
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

The NS Cloner saves multisite admins and developers TONS of time by cloning existing sites in a multisite network to a completely new site in a few seconds.

== Description ==

This is by far the easiest, fastest, and most user-friendly way you will ever create fully configured sites on your multisite networks. The NS Cloner will take any existing site on your WordPress multisite network and clone it into a new site that is completely identical in theme & theme settings, plugins & plugin configurations, content, pictures, videos, and site settings.

Everything is preserved and intelligent replacements are made so that the new site settings reflect your choices for the name and title, and have automatic URL replacements and other background updates to make sure the new site works exactly the same way as if you had taken the time to set it all up manually.

**Important:** this plugin *only* works with WordPress Multisite (although the pro version works for single sites as well). You will find its menu in your network administration dashboard (wp-admin/network).

= Typical Workflow for using the NS Cloner =
1. Set up 1 or more sites exactly the way you want your clones to start out.
2. Go to your Network Dashboard > NS Cloner.
3. Select the site you that want to clone, and enter the desired URL and title of the new site.
4. Clone away with one click!

Yes, it really is that easy.

= Primary Use Cases =
* Developers who host and manage multiple client sites in their own multisite environment - this will allow you to rapidly roll out new baseline sites with all your favorite standard plugins and configurations in place. No more tedious manual repetitive entry!
* Designers who want to be able to create several versions of sites to test and play with different theme designs in parallel, without wasting time with unnecessary duplication.
* Teams who want to have a quick way to set up staging sites for collaboration, or effortlessly duplicate content for regional versions of sites, etc.
* Organizations which provide "member" sites and want to be able to reduce the site spin up time to almost nothing.
* Affiliates that host numerous sites through multisite and are looking for a way to increase reach and decrease deployment times.

== Features ==

= Core Features =
* Copies an entire site in seconds
* Works in subdomain or subdirectory mode
* Copies all widgets, menus, and theme and plugin settings
* Copies all pages, posts, custom post types and taxonomies
* Copies all uploaded media files and associated data
* Works in the background to avoid timeouts or memory shortages on large sites
* You can close your tab without interrupting cloning, or stay and watch the progress live
* Advanced validation and preemptive issue detection
* Robust process logging to help with troubleshooting
* Hook-rich cloning pipeline for developers to extend
* Translation ready

= Pro Features =

For even more powerful functionality, [check out NS Cloner Pro](https://neversettle.it/buy/wordpress-plugins/ns-cloner-pro/). In addition to all the free core features, Pro includes:

* **Teleport** *(new)* - remote cloning power: clone a subsite to a remote network, or even teleport an entire multisite network to a remote location.
* **Single Site** *(new)* - gain the ability to clone standard single sites, not just multisite, and even clone between single and multisite or vice versa.
* **WP CLI Addon** *(new)* - easily copy sites directly from the command line.
* **Search & Replace** - perform unlimited, effortless custom search and replace on cloned content.
* **Table Manager** - easily manage exactly which database tables are cloned.
* **Users Cloning** - ability to clone all WordPress users and their permissions, or instantly create new users for cloned sites.
* **Presets** - save commonly used cloning settings as shortcuts for even ore time savings.

== Installation ==

1. Log in to your WordPress network as a multisite super admin and go to /wp-admin/network
2. Use the Dashboard > Plugins > Add New tools to install NS Cloner from the WordPress.org repository or install by uploading the zip file
3. Network Activate the NS Cloner through the 'Plugins' menu in WordPress
4. Access the NS Cloner from its main menu on the Network Dashboard (/wp-admin/network)

= Standard Precautions and Notes =
* Unlike some other tools, NS Cloner supports cloning the root site (ID=1). When cloning the root site, the Cloner will automatically exclude all global network WordPress tables (like wp_blogs) as well as global tables for some common network plugins like BuddyPress. It's impossible, though, for the Cloner to recognize every network-level table for every plugin out there, so it's possible that some network-level plugin tables could be copied by the Cloner incorrectly, which could result in issues, depending on the plugin. The table manager add-on included in pro is perfect for unique scenarios where you need total table-level cloning control.
* We always try to help (and you can see the proof of that in the plugin support forum here), but we cannot promise support to users for this free version, especially with issues resulting from non-standard environments.
* We have used the NS Cloner on production systems for years without issues. That doesn't mean your scenario won't find some new condition that could cause you some headaches. Unlikely, but always possible. We recommend getting familiar with it on a test system before you deploy it to a critical network.
* And for the love - backup your data. This plugin operates at the database level to work its magic. We've run it hundreds of times on our own sites and client sites, and tested it thoroughly. It's safe. But don't take our word for it.

== Frequently Asked Questions ==

= How do I contact support, provide feedback, or make a feature request? =
You can browse our Knowledge Base, add or vote on Feature Requests, or contact us with an issue at [support.neversettle.it](http://support.neversettle.it/)

= Where can I find more documentation? =
[See these articles](https://neversettle.it/documentation/ns-cloner/) for additional information on using NS Cloner.

= What exactly does the NS Cloner copy? =
The Cloner copies everything you need to have a totally identical twin site: all media uploads, posts, pages, custom post types, taxonomies, comments, menus, WordPress options, theme and plugin settings (including which ones are active).

Users and roles are not copied (that's a pro feature), and theme/plugin files are not copied because the same files are shared by the whole multisite network, so there's no need to copy them when cloning inside a network.

= Can I clone an individual site that's not part of a network (non-multisite)? =
That is a pro feature - so, yes! With Pro you can easily clone a single WordPress site to another single site. You can even clone a site out of a network to its own individual install or vice versa.

= What happens if my site is really large? =
You're in luck! NS Cloner V4 has new background cloning capability, so you should be able to clone a site of almost any size without running into a "white screen of death" from timeouts or memory limits. You can even close your browser and come back to check on it later without interrupting the clone!


== Screenshots ==

1. Main cloning options.
2. Cloning in progress.

== Changelog ==

= 4.0.4 - 2019.09.02 =
* Fix database handling for null values
* Fix fatal site creation error in pre-5.1 WordPress
* Fix error on servers that don't allow multiple SQL statements in one query
* Fix misc other bugs and plugin compatibility issues

= 4.0.3 - 2019.08.19 =
* Fix missing rows due to lost insert or incorrect row query
* Fix max_allowed_packet database error

= 4.0.2 - 2019.08.15 =
* Fix timing conflicts for cleanup tasks.
* Fix issue where process would keep running after manually cancelling.
* Rewrite row processing class for much better performance and fewer queries.
* Add fallback AJAX process dispatching for environments where background requests stall.
* Add queue batching for large tables.
* Improve debug logging.

= 4.0.1 - 2019.07.26 =
* Fix lock timing on background processes to prevent frozen or conflicting processes.
* Fix handling for SQL views - exclude from table cloning and create at end instead.
* Fix empty target site url caused by object caching on some servers.

= 4.0.0 - 2019.07.22 =
* Release all new rebuilt V4.

== Upgrade Notice ==

= 4.0.0 =
All new V4, with upgrades to everything - enhanced stability, power, interface and features.