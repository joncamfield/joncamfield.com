---
categories:
- mobile4dev
tags:
- sms
- mobile
- m4d
- m4change
- cell

title: After the SMS honeymoon? (Updated)
created: 1241203303
redirect_from: /blog/2009.05/after-the-sms-honeymoon-update.html

---
<em>Check out some updates -- props to @MobileActive!</em>

During the last breakout at the Mobile for Change (<a href="https://search.twitter.com/search?q=m4change">#m4change in twitter</a>, a good writeup by Development Seed's Will White: <a href="https://www.developmentseed.org/blog/2009/apr/30/recap-mobile-tech-4-social-change-barcamp">Recap of Mobile Tech 4 Social Change BarCamp</a> ) open conference yesterday, we began to get into some of the problems that had been bugging me all day.

During NDI's Ian Shuler's <a href="https://tinyurl.com/c5mn9w">presentation on the state of Mobile in Development</a> (especially in Election Observation) I twittered:

<blockquote style="twitter">what happens when govt catches up, blocks sms during unrest? we need p2p networks #m4change
<a href="https://twitter.com/joncamfield/status/1649285757">9:38 AM Apr 29th</a> from web</blockquote>

Now that I'm not constrained by 140 characters, let me unpack that a bit.

Repressive governments are getting smarter.  They've enjoyed the ability to censor, control and manipulate traditional media for quite some time now, and have been caught blindsided by the Internet and cell phones.  We cannot hope or expect that to continue.  We've seen the first, blunt reactions to this - shutting down SMS service during elections to prevent the spread of information, and during the #pman protests SMSs were severely throttled.  In #pman the protesters were able to continue exchanging information on their cellphone's data connections.  I wouldn't count on that working the next time around.

But it's unlikely that SMS would be totally cut off in a country for more than a few days around a big event, so why worry so much?

Because of course shutting SMS down temporarily is just the blunt response of a government that hasn't had time to do anything more devious.

Forcing all SMS messaging to run through a series of scans for keywords, tracking political dissidents using SMS to spread the word, and taking actions against people based on these types of logs would destroy the use of mobile phones - not only in the spread of democracy, but also in any form of activism that was not strictly in line with the current regime.

Due to the centralized structure of cell phone systems, scenarios that make China's Great FireWall look irrelevant are pretty easy to imagine even for a regime without much tech savvy.

So -- how can we fix this?

Encryption on cell phones has two big problems - it's not built in on most handsets and it's very clear that you're trying to hide something, which is just as bad as doing that something.  Unless encryption was built into the protocols and implemented by default, it's useless -- and even if it were implemented, the telco could probably still access the texts, so we're no better off than we were before.  Sure, end-to-end encryption would fix that, but key exchange and signing via SMS? I'd like to see a workable RFC on that.

I think the most valuable solution is a peer-to-peer mesh network that can carry voice, SMS, and data on it.  The downsides of these is that their range can be extremely limited by lack of density of users.

Turns out there are mesh phones out there, a Swedish startup called <a href="https://www.terranet.se/index.php?option=com_content&task=view&id=47&Itemid=87">TerraNet</a> (previously <a href="https://mobileactive.org/tagging/terranet">mentioned on MobileActive</a>) turns capable phones into mesh nodes:

<blockquote>The technology is simple: Terranet outfits a special Erricson phone with peer-to-peer wireless networking ability. In its pure form, there is no need for base stations, antenna installations or infrastructure. With this phone, a user can call and text anyone at no cost within two kilometers, or up to 20 kilometres in a mesh network.<br/ > (<em>Via MobileActive</em></blockquote>

<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a href="https://www.terranet.se/index.php?option=com_content&task=view&id=47&Itemid=87" ><img src="https://www.terranet.se/images/press/tn_cluster_lores.png" width="240" height="180" alt="TerraNet Mesh Phones" style="border: 2px solid rgb(0, 0, 0);" /><br /><span style="font-size: 0.9em; margin-top: 0px;">TerraNet Mesh Phones</span></a></div>

The trick of course is getting these mesh phones (or adding mesh capability into enough existing phones) rolled out in enough numbers to make a difference.  There are some clear use-cases in development for disaster-prone areas, areas without telco service (they could be a great business model for <a href="https://joncamfield.com/blog/2009.04/micro-telcos-business-models-f.html">micro telcos</a>), or as a low-cost phone + data connectivity tool.

However, there are quite a few barriers against this.  The price point is higher than your basic cell phone, and you have to have rapid local adoption for it to even work.  From a business side, it must fight against the existing install base of cell phones (and their providers).  The business plan for the network is itself hamstrung by the very power of the technology - in a mesh network, how do you charge for calls that you don't know about?

If however the mesh technology could be embedded on new phones as part of a disaster-mitigation scenario (even in the US, cell networks are notoriously overloaded during crisis), a powerful technology would find its way into daily usage that was immune to many of the censorship and oppression problems of centralized communications networks.

There's a project <a href="https://community.mit.edu/">Comm.Unity at MIT's Media Lab</a> that runs as a software piece on top of cells, PDAs, and laptops:

<blockquote>Comm.unity runs on mobile phones, PDAs, and regular old laptops and PCs, allowing them to easily communicate with each other and build networks of interactions for their users without the need for any centralized servers, coordination, or administration. </blockquote>

There's also <a href="https://www.inclusiva-net.es/fluidnexus/">Fluid Nexus</a> which <cite>is an application for mobile phones that is primarily designed to enable activists to send messages and data amongst themselves independent of a centralized cellular network</cite>

Fluid Nexus requires bluetooth, and for people to be within bluetooth range (though it is a store-and-forward style system), so it has its own limitations, but at the same time could be a powerful tool in the right situations.

It's a start.
<!--break-->
<strong>Updated content</strong>:

@MobileActive adds some others thinking along the same lines:

https://community.mit.edu/ : <cite>“Comm.unity” is a new communications platform being developed at the MIT Media Lab that would allow developers to easily create socially aware peer-to-peer applications for face-to-face interactions. Comm.unity runs on mobile phones, PDAs, and regular old laptops and PCs, allowing them to easily communicate with each other and build networks of interactions for their users without the need for any centralized servers, coordination, or administration."</cite>

https://www.inclusiva-net.es/fluidnexus/ : Fluid Nexus is an application for mobile phones that is primarily designed to enable activists to send messages and data amongst themselves independent of a centralized cellular network

Here's a video on Fluid Nexus:

<object width="400" height="267"><param name="allowfullscreen" value="true" /><param name="allowscriptaccess" value="always" /><param name="movie" value="https://vimeo.com/moogaloop.swf?clip_id=798016&amp;server=vimeo.com&amp;show_title=1&amp;show_byline=1&amp;show_portrait=0&amp;color=&amp;fullscreen=1" /><embed src="https://vimeo.com/moogaloop.swf?clip_id=798016&amp;server=vimeo.com&amp;show_title=1&amp;show_byline=1&amp;show_portrait=0&amp;color=&amp;fullscreen=1" type="application/x-shockwave-flash" allowfullscreen="true" allowscriptaccess="always" width="400" height="267"></embed></object><p><a href="https://vimeo.com/798016">Fluid Nexus Project Video</a> from <a href="https://vimeo.com/zeitkunst">Nick Knouf</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

### Archived Comments

* I think that mesh networking via phones with wifi is the way to go if you're designing software preemptively. Increasingly common, widely understood, and lots of open access points to piggy-back relays off of in case things get hairy. -- Mike Cotton Fri, 05/01/2009 - 15:48
  * I always thought that something like Fon.com with a mesh setup built in would be great. The problem, even in pretty dense urban areas, is having enough users with peer meshing enabled to make it work at all. -- Jon Mon, 05/04/2009 - 16:55
* Thanks, Jon, for the wrap. Enjoyed seeing your demo of FrontlineSMS/OLPC. -- Paul Wed, 05/06/2009 - 15:56
* thank you Jon for video and your report i following you ;p -- mr@t3awn.com Sat, 08/29/2009 - 00:21
