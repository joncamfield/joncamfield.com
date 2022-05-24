---
excerpt: "<p><em>This is the continuation of my journal on getting mapping to work
  for Global Youth Service Day in Drupal, which <a href=\"http://www.joncamfield.com/blog/2008/10/how_i_made_a_map_for_global_yo.html\">starts
  with an overview of maps and drupal</a>, and continues <a href=\"http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html\">with
  a discussion of modules</a>.</em></p>\r\n\r\n<p>So now we have the basic setup and
  are ready to start on the map - placeholders for content, maps, and actual content,
  and it's time to forge ahead with improving the user experience and information
  architecture (at the same time, even!).</p>\r\n\r\n<p>I also just came across another
  blog article at around the same level of detail that covers other aspects of Drupal,
  which I haven't touched on much here for a more articles-rich site.  Check it out:
  http://dejitarob.wordpress.com/2007/11/26/how-i-used-drupal-to-build-tampa-bay-indymedia/
  .  Along similar lines, I stumbled across a series by IBM that gives a surprisingly
  clear overview of the next level in to Drupal geekery, without flooding you with
  information: http://www.ibm.com/developerworks/ibm/library/i-osource5/</p>\r\n"
categories:
- ict4d
- web 2.0 and f/loss
tags:
- map
- drupal
- gysd

title: 'Drupal and Maps III: Getting Dirty.'
created: 1227090660
---
<p><em>This is the continuation of my journal on getting mapping to work for Global Youth Service Day in Drupal, which <a href="http://www.joncamfield.com/blog/2008/10/how_i_made_a_map_for_global_yo.html">starts with an overview of maps and drupal</a>, and continues <a href="http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html">with a discussion of modules</a>.</em></p>

<p>So now we have the basic setup and are ready to start on the map - placeholders for content, maps, and actual content, and it's time to forge ahead with improving the user experience and information architecture (at the same time, even!).</p>

<p>I also just came across another blog article at around the same level of detail that covers other aspects of Drupal, which I haven't touched on much here for a more articles-rich site.  Check it out: http://dejitarob.wordpress.com/2007/11/26/how-i-used-drupal-to-build-tampa-bay-indymedia/ .  Along similar lines, I stumbled across a series by IBM that gives a surprisingly clear overview of the next level in to Drupal geekery, without flooding you with information: http://www.ibm.com/developerworks/ibm/library/i-osource5/</p>
<!--break-->
<h3>Create custom content types and taxonomies for the events</h3>
<p>I created one content type with required location information for the events, and a few others for participant roles (to link in organizations running events in a more controlled fashion than a free text field).  I'm planning to use node_import to pull those in from our database (and by database, I of course really mean excel spreadsheets).  I set it up so that any logged-in user can add content to these types, but it won't be automatically published (allowing for some oversight and cleansing of poorly inputted information).  This step lets me sort, manage, and delete items with better precision, which becomes Really Useful if you're going to run some batch imports - the first few I can almost guarantee will be wrong in some insidious ways.</p>

<p>Then I created a few taxonomies to support further categorization of my events (did they receive grant money to run the event?  Did the event fit into one of the MDG categories?? ), but this isn't strictly necessary (though it can add more dimensions to searching and map presentations once you get into the views, below).  It's a LOT easier to do this well, ahead of time, than to go back and fix it later.</p>

<p>Taxonomies (and the difference between Content Types and Taxonomies, and taxonomies internally) can get hairy to grok.  My brain understands taxonomies best as super-configurable dimensions of data that you can apply pretty flexibly to your content.  Content Types are one dimension that is specifically useful to manage user permission and back-end content management with (logged in users can post X, but only administrators can post Y, for example).  You've got to balance the tempation to over-taxonomize your site with the user experience (how many drop-downs, multi-selects and free tagging fields do they really want to deal with every time they create content??).  You can have a taxonomy apply to only specific content types, which I found handy with the map, as there was a set of categories really useful to the map data, but I wouldn't want to force them on blog entries.</p>

<h3>Testing, 1...2...3...</h3>

<p>Finally, I imported last year's event data, just so I could see how the map works.  you can always go through and delete it all if you must, later (before the site goes live, hopefully!).  Note: using the latest version of the location module seems to muck with the node_import module's way to figure out which fields it can import into - see http://drupal.org/node/307677 for a potential workaround.  Lesson: Be ready for some oddities when using beta releases!</p>

<p>Actually, I got on #drupal and #drupal-support (chat rooms on irc.freenode.net) and ran into the head Locations module developer who pointed me to a code patch that fixed all my problems.  It's things like that that make me love the open source culture.</p>

<p>Even so, as the Location is in the middle of a massive code change that throws these errors once in a while when you're setting up filters based on location information.  Right now I recommend watching the forums - most of it works, and it will all work a lot better than the previous stable release, you'll just have to be careful around some of the rough edges.</p>

<p>It took me a few rounds of "import, field-match, peek at the map, delete it all, start over again" before I got to a mostly-happy point with the imported data.  If you're starting fresh, it's a lot easier, and you don't have to worry about the various problems I was encountering with some bad formatting errors and inconsistent data in the import file.  Instead, you get to go through the Create Content tool that your end users will be using to post a few sample entries.</p>

<h3>A note on Gmap configuration and "geocoding"</h3>

<p>Geocoding is the art of matching an address to a Latitude/Longitude on the map, and it works best in the USA and a few other nations.  GMap provides a (somewhat hard to use) tool that lets users click a map to select their location, or you can point them to a third party map tool that walks them through finding their Lat/Long to input back in your site.  If you find a better solution - let me know!</p>

<p>Once you have a few map points in, click on the "Node Locations" navigation option and they should show up -- your first map!</p>

<p>Next up: slicing and dicing the map  to show custom fields and specific types of data, not just everything!</p>
