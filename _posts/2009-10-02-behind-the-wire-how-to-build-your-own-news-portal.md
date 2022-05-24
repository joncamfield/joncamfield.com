---
excerpt: "<div style=\"align:right\"><img src=\"http://servicewire.org/sites/default/files/logo.png\"
  alt=\"ServiceWire Logo\" border=\"0\" /></a></div><a href=\"http://www.ServiceWire.org\">ServiceWire.org</a>
  is a refreshed version of a news system that's been part of YSA's servenet.org toolset
  for years.  In fact, when servenet.org was launch in the mid-nineties (1996 in fact)
  its motto was \"Our Content in Youth Info\" - a few years ahead of its time in terms
  of \"Web 2.0\" concepts or peer-generated content.\r\n\r\nIn late 2008 I decided
  it was time to bring ServiceWire up to date with current technologies.  It still
  got a smattering of news and press release submissions from the field, but it was
  no longer the source of news and knowledge about what was happening in the service
  movement.\r\n\r\nAt its heart, ServiceWire is very simple - it takes content from
  the service field and collects it all in one place, making it easy to follow, comment
  on, and explore trends.\r\n\r\nRead on to learn all about how it works, how you
  can take greater advantage of it, and how you can make your own version of it!\r\n"
categories:
- tinkering
- web 2.0 and f/loss
tags:
- drupal
- servicewire
- rss
- ictdev.org ictdev
- pulse
- wire
- howto
- managingnews
- developmentseed
- feedapi
- xml

title: 'Behind the Wire: How To build your own news portal'
created: 1254506845
---
<div style="align:right"><img src="http://servicewire.org/sites/default/files/logo.png" alt="ServiceWire Logo" border="0" /></a></div><a href="http://www.ServiceWire.org">ServiceWire.org</a> is a refreshed version of a news system that's been part of YSA's servenet.org toolset for years.  In fact, when servenet.org was launch in the mid-nineties (1996 in fact) its motto was "Our Content in Youth Info" - a few years ahead of its time in terms of "Web 2.0" concepts or peer-generated content.

In late 2008 I decided it was time to bring ServiceWire up to date with current technologies.  It still got a smattering of news and press release submissions from the field, but it was no longer the source of news and knowledge about what was happening in the service movement.

At its heart, ServiceWire is very simple - it takes content from the service field and collects it all in one place, making it easy to follow, comment on, and explore trends.

Read on to learn all about how it works, how you can take greater advantage of it, and how you can make your own version of it!
<!--break-->
<h2>The birds and the feeds: where news comes from</h2>

<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><img src="http://tools.ysa.org//logos/reflection250/rss_reflection.png" alt="Large RSS Symbol"></div>Let's start with the "takes content from the service field" part. ServiceWire draws from a variety of news sources and RSS feeds - Google scans for keywords, feeds from volunteer and service blogs, key service and service-learning websites such as Youth Service America, ServiceLearning.org, and <a href="http://servicewire.org/wire/sources">many other websites</a>.  ServiceWire also has a blogging system for more in-depth commentary on current service and volunteer events. 

<em>Wait, what are these feeds you're talking about?</em> Learn about feeds (RSS) at my <a href="http://joncamfield.com/blog/2008/08/rss_is_my_favorite_web_magic.html">RSS is my favorite web magic</a> blog entry.

Guests can use the <a href="http://servicewire.org/contact">contact page</a> to suggest other news feeds, or <a href="http://servicewire.org/contribute ">contribute individual items</a>, which get screened to prevent spam.

A third source of content is YSA's <a href="http://servicewire.org/nsb/all">National Service Briefing</a>, which gets archived on ServiceWire. The Briefing is a weekly email publication which highlights current information such as effective practices, funding, awards, legislation, corporate initiatives, calendar events, and "profiles in service" - stories of youth leading innovative service initiatives.

Stories from the NSB are edited by Michael Minks at Youth Service America. You can suggest a story for the NSB by emailing NSBinfo@ysa.org.

Youth Service America staff also contribute news, links and stories to make sure that the National Service Briefing and ServiceWire are the definitive source for service news. Contact wire@servicewire.org if you're interested in lending a hand.

<h2>Where the news goes</h2>

As a resource for the field, ServiceWire also lets you subscribe to feeds coming out of this "filter" of news. Look for the RSS icon: <img src="http://joncamfield.com/misc/feed.png" alt="RSS Icon" /> on pages to subscribe using your favorite RSS reader, or even via email using http://www.rssfwd.com .  My personal favorite feature is the <a href="http://servicewire.org/wire/customsearch">Custom Search tool</a> that lets you put in keywords to search for, and presents you with an RSS feed you can subscribe to - want to keep tabs on <a href="http://www.GYSD.org">Global Youth Service Day</a>?  Simply <a href="http://servicewire.org/wire/customsearch?wiresearch=GYSD+%22global+youth+service+day%22">add some keywords and go</a>. 

ServiceWire's main outbound news feed can also be embedded in your site via a simple <a href="http://www.widgetbox.com/widget/servicewire">widget</a>, and you can follow its stories at its <a href="http://www.twitter.com/ServiceWire">@ServiceWire twitter account</a>.

<h2>Site Organization</h2>

<div style="float: right"><img src="http://farm4.static.flickr.com/3642/3387985048_436dcb9375_m_d.jpg"><br /><span><em>Illustration by <a href="http://www.flickr.com/photos/xjara69/3387985048/">Jarek Pelczynski on Flickr</a></em></span></div>The National Service Briefing is divided into clear sections and carefully edited to present a crisp and clear overview of the top service stories each week. The ServiceWire is a much less controlled environment, due to the incredible scale and scope of community service and service-learning around the world. We are working on segmenting the news gathered through the wire into natural categories (beyond being able to read them by their source).  

This is all done with the Swiss Army Knife of Drupal modules, Views.  Views lets you search and filter content through URL variables (we use dates in servicewire, so this story from BeTheChange about the Learn and Serve Challenge is posted at http://servicewire.org/content/20090925/wire/bethechange/Next-Service-Calendar-National-Learn-and-Serve-Challenge-Oct-5-11 (the pathauto and token modules let you make URLs based around information from the article).  Views is set up to present all the ServiceWire content from that same day at http://servicewire.org/content/20090925/wire (NSB content follows the same rule, but only shows up on the days the NSB is published, like here: http://servicewire.org/content/20090924/nsb ).

<h2>Getting (more) Technical</h2>

ServiceWire runs atop Drupal and is powered primarily by the <a href="http://drupal.org/project/feedapi">FeedAPI module</a>, sponsored by the DC-area Drupal wizards at <a href="http://developmentseed.org/">DevelopmentSeed</a>.  FeedAPI does the work to take RSS feed items and re-package them at ServiceWire.

ServiceWire is hosted for (almost) free by DreamHost -- DreamHost provides free business hosting for nonprofits, ServiceWire runs on their (still very affordable) Virtual Servers due to its at-times heavy loads. It runs on the Drupal content management system using all open source, volunteer-created tools.

As mentioned above, the core tools are FeedAPI (and FeedAPI_Mapper) and Views.  Pathauto plays an important role in syncing imported content URLs to what the Views are set to offer through their arguments (variables).  A few of the tabs (like the grants tab) use Views filters to narrow down stories by keywords, and Custom Search page exposes that filter to let the user choose their own keywords.  ServiceWire uses Captcha and Mollom to reduce spam, and AddThis to enable viral spread of stories by users who want to post to their twitter/facebook/etc. accounts.  We use Elysia Cron and/or poormanscron to help keep the site updating regularly when it gets bogged down with too much news at once, though the latest versions of FeedAPI have new features governing how often each feed gets checked which reduce this problem greatly. We also have some print-to-pdf and email modules thrown in.  All of this is open source, and now you even have the blueprint to put it together yourself!

<h2>Looking Forward</h2>
ServiceWire will forever be about volunteering and service with related news.  It will never be about, say, emerging thoughts on how to use technologies like computers and cell phones in international development contexts.  The beauty of ServiceWire is that it scales horizontally, not vertically.  If you want vertical scale in news aggregation, you are either <a href="http://alltop.com/">AllTop</a> or you're <a href="http://www.google.com/reader">Google Reader</a> (or you have some really stiff competition).  The Achilles heel of vertical scale is you lose the community feel of a cause-centric site.  It's why CNN doesn't compete with your local news channel.

<div style="float:right"><a href="http://ictdev.org"><img src="http://ictdev.org/misc/ictdev.png" width="200" border="0" alt="ICTDev logo" /></a></div>I've already gone and duplicated the pieces behind ServiceWire at <a href="http://www.ICTDev.org">ICTDev.org</a>, which covers technology for development.  It has a few extra (and experimental) bells and whistles - an <a href="http://i.ictdev.org/">iPhone version</a>, a fancy "carousel" of recent news, and the fivestar voting system to rate popular content.  Look for those features to make their way to ServiceWire as the bugs get ironed out!
