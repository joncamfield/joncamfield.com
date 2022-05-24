---
excerpt: "<p><em>This is the continuation of my journal on getting mapping to work
  for Global Youth Service Day in Drupal, which <a href=\"http://www.joncamfield.com/blog/2008/10/how_i_made_a_map_for_global_yo.html\">starts
  with an overview of maps and drupal</a>, and continues <a href=\"http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html\">with
  a discussion of modules</a>, then talks about <a href=\"http://www.joncamfield.com/blog/2008/11/drupal_and_maps_iii_getting_di.html\">getting
  content into the map.</a></em></p>\r\n\r\n<p>Remember back in <a href=\"http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html\">Part
  II where I mentioned the Views and Panels module</a>?</p>\r\n\r\n<p>Views gives
  you very precise control over what shows up on new maps you can show up.  Even better,
  use can create \"arguments\" that can be passed through the URL to further define
  what shows up.  For example, I created a view whose base URL was /gysd/map/ -- if
  you go there, you get a listing of years to choose from (do you want to see events
  from GYSD 2008?  GYSD 2009?)  If you click on 2008, the url is now /gysd/map/2008
  - and you see all the events for that year.  I then created some other map options
  to list by country, state, and so on, so there's another path that goes like this:
  /gysd/map-by-location/2008/us/FL .  If I cut that one off at 2008/, I'd see a listing
  of all the countries I had data for.  If I cut it at us/ , I'd see all the regions
  (states) with data.  You could also set a map up with zip codes, taxonomies, and
  so on.  Drupal 6's Views2 is an order of magnitude more powerful that Views1, and
  alone it's a reason to upgrade to D6.</p>\r\n\r\n<p>To create a map view, you have
  to first (after installing the views modules above, and creating a new view) select
  GMap View from the Page view set of options (under View Type).  This enables the
  map functionality.  I put information into the Header section to guide users in
  the navigation process.</p>\r\n"
categories:
- ict4d
- tinkering
- web 2.0 and f/loss
tags:
- map
- drupal
- gysd

title: 'Drupal Mapping IV: Filtering and Customization of the Map'
created: 1230287400
---
<p><em>This is the continuation of my journal on getting mapping to work for Global Youth Service Day in Drupal, which <a href="http://www.joncamfield.com/blog/2008/10/how_i_made_a_map_for_global_yo.html">starts with an overview of maps and drupal</a>, and continues <a href="http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html">with a discussion of modules</a>, then talks about <a href="http://www.joncamfield.com/blog/2008/11/drupal_and_maps_iii_getting_di.html">getting content into the map.</a></em></p>

<p>Remember back in <a href="http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html">Part II where I mentioned the Views and Panels module</a>?</p>

<p>Views gives you very precise control over what shows up on new maps you can show up.  Even better, use can create "arguments" that can be passed through the URL to further define what shows up.  For example, I created a view whose base URL was /gysd/map/ -- if you go there, you get a listing of years to choose from (do you want to see events from GYSD 2008?  GYSD 2009?)  If you click on 2008, the url is now /gysd/map/2008 - and you see all the events for that year.  I then created some other map options to list by country, state, and so on, so there's another path that goes like this: /gysd/map-by-location/2008/us/FL .  If I cut that one off at 2008/, I'd see a listing of all the countries I had data for.  If I cut it at us/ , I'd see all the regions (states) with data.  You could also set a map up with zip codes, taxonomies, and so on.  Drupal 6's Views2 is an order of magnitude more powerful that Views1, and alone it's a reason to upgrade to D6.</p>

<p>To create a map view, you have to first (after installing the views modules above, and creating a new view) select GMap View from the Page view set of options (under View Type).  This enables the map functionality.  I put information into the Header section to guide users in the navigation process.</p>
<!--break-->
<p>In Fields, you get the option of what data you pass to the view.  Think of views as lenses that you can see your whole site through, but best used to explore a few pieces of data from your site in a controlled way with.  At the very least, you have to pass the Node Title and the latitude and longitude information to the map view (or it won't know what to place or where to place anything).  You can add more later, and control what is actually visible to the user using custom CSS code (I hid the lat/long numbers).</p>

<p>Arguments are what I discussed above.  Start out with none and add more as you want to customize your map and the user's path and ability to view specific subsets of your map data.</p>

<p>Filters are super important - this is where you tell the view what content types (or taxonomies, etc.) to show.  I created a filter to only show the "GYSD Event" content type.  Also highly recommended is filtering on published content only if you have any workflow set up.  You can also expose filters to the user to allow them to filter in real time on taxomonies (or whatever).  Right now, I'm in the process of working on this - where are arguments and url paths more useful, and where are user-exposed filters more useful?</p>

<p>If views are meta-approaches to looking at content, panels are a meta-approach to looking at and presenting views (or lower-level content, of course).  You can combine maps and lists within the same panel kind of like being able to present multiple web-pages linked together inside of one.  You have to first create panes for the panel that translate the panel options into options for each pane.  For example, the view could have a url like map/2008/us/TX to show 2008-only events in Texas, and the panel url could be simply map/tx - you'd need to tell the pane what arguments from the panel (argument #1 is tx) correspond to which arguments for the view (the view expects the third argument to deal with states, so you have to set the first and second to static (2008 and 'us'), and then tell the pane to translate the first panel argument into the third view argument.  Make sense?  Great!  Huh?  No?   Well, yeah. It's a bit complex, but remember that you're basically having one web page with one set of arguments and filters talk to any number of separate views - each previously their own page with their own filters and arguments.  The panes setup lets you translate between them without having to make all your views specifically formatted in the exact same way.  It's the standard geek problem - in making something very flexible and easy, you end up with a very complex sounding system.  I find it easiest to understand these decisions after having understood the problem they're meant to solve.</p>

<p>I'll continue this discussion after I can get some sample data in from 2008 (node_import remains unavailable for D6) or new data for 2009 events.  Happy holidays and happy hacking!</p>
