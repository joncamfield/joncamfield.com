---
excerpt: "<p><strong>Series</strong>: <em><a href=\"\">Overview</a> | <a href=\"https://www.joncamfield.com/blog/2008.10/drupal_and_maps_ii_modules_in_1.html\">Modules</a>
  | <a href=\"https://www.joncamfield.com/blog/2008.11/drupal_and_maps_iii_getting_di.html\">Structure
  and Taxonomies</a> | <a href=\"https://joncamfield.com/blog/2008.12/drupal_mapping_iii5_moving_up.html\">On
  Drupal 6</a> | <a href=\"https://joncamfield.com/blog/2008.12/drupal_mapping_iv_filtering_an.html\">Functionality</a></em></p>\r\n
  \r\n<p>Drupal by itself is pretty powerful, but where it really shines is when you
  start plugging in the modules which have been developed for it.  There are hundreds
  (if not thousands), and the first mistake I made on my first Drupal install was
  to just start clicking away before I'd learned the ropes.  Luckily, this is what
  sandbox installs are made from, so a few database drops and folder deletions later
  I could start from scratch (again).</p>\r\n\r\n<p>To get this all working, I now
  present you with the modules I activated or installed for the map project:</p>"
categories:
- ict4d
- web 2.0 and f/loss


title: 'Drupal and GYSD Maps II: Modules in Play'
created: 1224788541
---
<p><strong>Series</strong>: <em><a href="">Overview</a> | <a href="https://www.joncamfield.com/blog/2008.10/drupal_and_maps_ii_modules_in_1.html">Modules</a> | <a href="https://www.joncamfield.com/blog/2008.11/drupal_and_maps_iii_getting_di.html">Structure and Taxonomies</a> | <a href="https://joncamfield.com/blog/2008.12/drupal_mapping_iii5_moving_up.html">On Drupal 6</a> | <a href="https://joncamfield.com/blog/2008.12/drupal_mapping_iv_filtering_an.html">Functionality</a></em></p>
 
<p>Drupal by itself is pretty powerful, but where it really shines is when you start plugging in the modules which have been developed for it.  There are hundreds (if not thousands), and the first mistake I made on my first Drupal install was to just start clicking away before I'd learned the ropes.  Luckily, this is what sandbox installs are made from, so a few database drops and folder deletions later I could start from scratch (again).</p>

<p>To get this all working, I now present you with the modules I activated or installed for the map project:</p>

Core Optional modules enabled
<ul>
<li>Blog/BlogAPI (if you want blog entries, and to enable usage of third party tools like the Flock Browser as blog-writing clients)</li>
<li>Taxonomy (This may or may not be actually "optional"</li>
<li>Profile (If you want user profiles)</li>
<li>Menu (Handy for working with your menus / user experience)</li>
</ul>
Modules downloaded and installed
<ul><li>Location - (Location, Gmap, Gmap location, Gmap Views Integration -- you can't have a map without locations and a map provider)</li>
<li>Event (if you want the Map points to also have start/end dates or (separately?) provide calendar info)</li>
</ul>
Advanced modules (do these later!)
These are a few modules I used to extend what I had created with the above tools to a more final product.  If you're new to this stuff like I was, it's definitely too much to bite off at once -- I found the learning curve much more agreeable to deal with slowly and need-driven.  
<ul>
<li>Node Import (if you have CSVs of events to batch-import)</li>
<li>Views  (Views, Views RSS, Views Theme Wizard, Views UI -- more about views and panels later)</li>
<li>Location Views -- you can't have a map without this stuff!)</li>
<li>Image (if you want users to attach photos)</li>
<li>Panels (panel pages, mini panels, panel nodes, views panels)</li>
<li>CCK (Fieldgroup, Text, Option Widgets; only if you want to add and filter on custom fields outside of what the above modules provide - try it without first; K.I.S.S.)</li>
</ul>
Some General Drupal Modules (Which I just think are useful)
These are some things I just like to add to most sites I create in Drupal to create some base-level tools and tracking.
<ul>
<li>Adsense (basic) (make money through Google Ads)</li>
<li>Google analytics (track pageviews)</li>
<li>Share (easy javascript applet that makes it easy for visitors to copy content to their Facebook / social bookmarking / etc. sites)</li>
<li>Spam (Great tool for detecting and managing spam)</li>
<li>Captcha (Used to be the best tool to filter out spammers, still helps, but annoys many users</li>
<li>Community Tags; Tagadelic (Fun tagging tools)</li></ul>

<p>After installing all those, you'll have to do a bit of initial work - setting up your domain's Gmap API Key and Analytics settings, default GMap preferences (autozoom, and open the info window when a marker is clicked, in my case).  Make sure you click through the administration-by-module page and at least peek into the settings for all these modules to give you an idea of what can and can't be tweaked from the module settings page.  Captcha requires you to upload some fonts to work well, and needs access to a decent image library (usually not a problem).  Spam needs some tweaking.</p>

<p>This is a good time to take a short jaunt through all of Drupal, post some content, play and learn about URL shortcuts, menus, and blocks, and how they work together on your pages.  You might also check out a few of the different Drupal themes (many good themes are available for free), and generally get your feet wet in Drupal.  I for example added the Google Translate applet (as a block) so that any page could be translated through Google's Translation tool. </p>
