=== Media Temple Server Status ===
Contributors: andrewryno
Donate link: http://andrewryno.com/plugins/media-temple-server-status/
Tags: mediatemple, server, stats, statistics, ve, mt
Requires at least: 3.3
Tested up to: 3.3.1
Stable tag: 1.2

This plugin places a widget on the WordPress admin dashboard giving you a brief overview of your (mt) server status.

== Description ==

Do you use mediatemple and wish you could view your server status directly from your WordPress installation? This plugin
adds a widget to your admin dashboard which gives you the ability to see your memory and CPU usage as well as the 
number of processes currently running on your server (more to be added soon). It displays these statistics using the 
Google Charts API to present them in the most friendly way possible.

== Installation ==

1. Upload the `mediatemple-server-status` folder to `wp-content/plugins/`
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Visit the options panel (located under Settings) and input your (mt) API key and select a service

To find your API key (or create one) visit https://ac.mediatemple.net/api/ when logged into your mediatemple account.

== Frequently Asked Questions ==

= When will you be adding more data points (e.g. loads, different date ranges, etc.) =

The goal is to have plenty more data available in the next version. The mediatemple API gives access to plenty more 
data but the Google Charts API makes it difficult to display all this data with the correct units. Once I figure 
out what the best way to handle them are, I will add in the extra data points. I am also planning to add in multiple
date ranges as well.

== Screenshots ==

1. A view of an example chart generated from the plugin showing the three different data points.
2. A view of the options page where the API key and service are managed.

== Changelog ==

= 1.2 =
* Deleted actual API wrapper file.
= 1.1 =
* Removed external API wrapper and all cURL dependency since it's not enabled on all servers. Now uses `file_get_contents()` which will work on more/all servers and much faster with less memory usage.
= 1.0.1 =
* Added a check to see if cURL is installed on the server since it is used for the (mt) API.
= 1.0 =
* First Release

== Upgrade Notice ==

= 1.0 =
No upgrade notices (first release).