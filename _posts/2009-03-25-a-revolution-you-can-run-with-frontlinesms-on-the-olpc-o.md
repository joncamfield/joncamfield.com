---
excerpt: "By attaching a computer (Linux, Mac, or Windows) to a cell phone with a
  data cable and installing his (free, open source) software, FrontlineSMS, that computer
  is turned into a messaging hub; sending and receiving text messages via the cell
  phone to hundreds of contacts."
categories:
- olpc
- mobile4dev
- hactivismo
- human rights
tags:
- sms
- mobile
- frontlinesms
- africa
- kiwanja
- ken banks

header:
  overlay_image: /assets/images/olpc-frontlinesms.jpg
  overlay_filter: 0.5
  teaser: /assets/images/olpc-frontlinesms.jpg


title: 'A revolution you can run with : FrontLineSMS on the OLPC \o/'
created: 1238003261
---
<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a href="http://www.flickr.com/photos/kiwanja/"><img alt="FrontlineSMS logo" src="http://farm4.static.flickr.com/3101/3170328164_5508f9f57d_m.jpg" style="border: 2px solid rgb(0, 0, 0);" /><br /><span style="font-size: 0.9em; margin-top: 0px;">FrontlineSMS Empowers: \o/ !</span></a></div> I recently saw Ken Banks present at a local <a href="http://www.irex.org/programs/techseries/summaries/0319_banks.asp">speaker series run by IREX</a>.  He gave an updated version of <a href="http://frontlinesms.ning.com/video/video/show?id=2052630:Video:8971">this presentation from POPTech</a>, on the power of mobile phones in citizen empowerment, NGO communication, and a host of other amazing stories of using the available, appropriate technology in remote and rural locations which are often off-grid and without Internet access.  By attaching a computer (Linux, Mac, or Windows) to a cell phone with a data cable and installing his (free, open source) software, FrontlineSMS, that computer is turned into a messaging hub; sending and receiving text messages via the cell phone to hundreds of contacts.

That's pretty amazing.  Three reasonably available pieces of hardware and you have a tool to send alert messages out, receive election monitoring information through, or communicate with field medical workers to coordinate and track supplies and treatment information.  Or track corruption.  Or report human rights violations.  Or share news and tips in places where the media is not independent, as one of the FrontlineSMS success stories shows:

<div style="float: left; margin-right: 10px; margin-bottom: 10px;"><a href="http://www.flickr.com/photos/kiwanja/"><img alt="FrontlineSMS logo" src="http://farm4.static.flickr.com/3108/3169852589_e32609067b_o.jpg" style="border: 2px solid rgb(0, 0, 0);" /><br /><span style="font-size: 0.9em; margin-top: 0px;">The FrontlineSMS Logo</span></a></div> <blockquote>"Based in Africa in a country where broadcast technology is controlled by a dictatorial government, this software has enabled me to communicate with the public at large. I am able to run my project without drawing unnecessary attention to myself—a good thing in this neck of the woods."
— Anonymous</blockquote>

Of course, you still have to worry about the cellular network itself.  Is the cell provider snooping messages and tracking approximate locations of where they're coming from, perhaps at the behest of the government?  Perhaps for some of these situations, it would be convenient to have a very mobile, mobile engagement system.  One that's pretty rugged, lightweight, innocent-looking, with a a low power draw and decent battery life, rechargeable from off-grid sources, and a few spare USB ports?
Know any computer that might fit that bill?
<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a href="http://www.flickr.com/photos/joncamfield/2600960763/" title="Solar Powered OLPC"><img src="http://farm4.static.flickr.com/3003/2600960763_078f525c11_m.jpg" alt="Solar Powered OLPC" style="border: 2px solid rgb(0, 0, 0);" /><br /><span style="font-size: 0.9em; margin-top: 0px;">Solar Powered OLPC</span></a></div>

<div style="float: left; margin-right: 10px; margin-bottom: 10px;"><a href="http://www.flickr.com/photos/joncamfield/3404569960/" title="FrontlineSMS loading on the OLPC by joncamfield, on Flickr"><img src="http://farm4.static.flickr.com/3539/3404569960_bdf8b05505_o.jpg" alt="FrontlineSMS loading on the OLPC" style="border: 2px solid rgb(0, 0, 0);" /><br /><span style="font-size: 0.9em; margin-top: 0px;">FrontlineSMS loading on the OLPC</span></a></div> FrontlineSMS, with a bit of hassle, runs on the OLPC XO.  I haven't gotten it working in Sugar, but it is happy enough in the <a href="http://www.olpcnews.com/forum/index.php?topic=4053">Ubuntu build for the OLPC</a>.  FrontlineSMS is written in Java, so a bit of software updating was in order, and I'm still having a few glitches with the system.  I also haven't yet sourced a cell phone that I can connect to the XO and that I can use to send messages, but I don't see why that would cause any more hassle on the XO than on anything else, presuming you can get a USB data cable.

A bonus benefit of running FrontlineSMS from a USB stick or SD card is that the XO will cheerfully boot up into standard Sugar if you eject (and conceal or destroy) the boot media.

<br clear="all" />For the techies and programmers, here's what's up:

Sugar - I think it should work fine in Sugar.  I'm suspecting that it's not talking with the GUI correctly.

<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a href="http://www.flickr.com/photos/joncamfield/3403759601/" title="FrontlineSMS running on the OLPC by joncamfield, on Flickr"><img src="http://farm4.static.flickr.com/3423/3403759601_07a726acd1.jpg" width="250" height="188" alt="FrontlineSMS running on the OLPC" style="border: 2px solid rgb(0, 0, 0);" /><br /><span style="font-size: 0.9em; margin-top: 0px;">FrontlineSMS on the OLPC</span></a></div>
In Ubuntu-on-XO (but not Ubuntu on my Dell) - trying to add an SMS Internet service crashes it, immediately, every time.  It seems to be a failure of the EventQueue, or at least that's the active thread at crash.  IANAJP (Java Programmer).


### Archived Comments

* Great to hear you got FrontlineSMS working on OLPC. I'm sorry to hear it doesn't work on Sugar. I've not had any direct experience with an OLPC (in fact, I don't know anyone who has one), but according to the Sugar wiki, it doesn't play too nice with Java. Maybe if you send one over to the UK we could take a closer look ;-) As for the issues with internet SMS services on Ubuntu, I'm surprised! If you submit your logs and let us know when you've done it over at the FrontlineSMS forum we'll take a look at the problem. Keep us posted how you get on connecting a real phone, too. -- Alex Anderson, FrontlineSMS developer Thu, 04/02/2009 - 05:41
 * Hah! If I had OLPCs to give out believe you me Frontline folks would have 'em; I'm not connected to OLPC except as an avid user and writer over at www.OLPCNews.com (which is rarely OLPC's favorite blog...) I got mine through G1G1 in 2007/8, and there are a few on eBay and probably some users groups over on your side of the pond as well (peek into OLPCNews.com/forum perhaps?) I'll loop back around and post on the FrontlineSMS forum this weekend hopefully; it's probably a java hiccup and not a Frontline hiccup -- Jon Fri, 04/03/2009 - 14:14
 *  There aren't many XOs on eBay in UK actually; I should probably try those forums. Have you had any more progress with FrontlineSMS yet? -- Alex Anderson Thu, 04/23/2009 - 12:09
 * I've been totally swamped with the tech side of Global Youth Service Day the past month; hope to get back to fidgeting with FrontlineSMS on the OLPC next month! -- Jon Fri, 04/24/2009 - 15:15
  * A few of the US eBay auctioneers will ship overseas (for additional cost, of course) but there seem to be a lot of XOs selling for ~200 USD with free US shipping. Also check the forums out as there is an active EU OLPC community which may know of some spare XOs that could go to a good cause. -- Jon Mon, 04/27/2009 - 16:48
