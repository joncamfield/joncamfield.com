---
categories:
- web 2.0 and f/loss
- human rights
- decentralization
header:
  overlay_image: /assets/images/cylon-evolution-poster-via-io9.jpg
  teaser: /assets/images/cylon-evolution-poster-via-io9.jpg
  caption: "Poster of cylon models via io9"
excerpt: "This has all happened before. This will all happen again."
title: Cylons, Open Source, and Security
created: 1475849162
---
<h3>The Lock-in / Break-out Cycle</h3>

"This has all happened before. This will all happen again." - a refrain from the rebooted Battlestar Galactica science fiction series that is painfully accurate in the software world. This is not always ideal, but it is reality.

We have a serious problem with vendor lock-in -- and this is an old, constantly recurring problem in technology.  In the dark ages of the web, there were first a gazillion individual websites - then a tendency towards a few online blogger/journaling communities (LiveJournal? GeoCities? Blogspot?). As these imploded, a new round of self-hosted blogs emerged (better! more powerful!).  Currently there's another return towards centralized blogs (Tumblr, Medium)  We have problems where Google complies with (or is forced to comply with) government requests for personal data. We have a huge problem where the business model of the vast majority of the Internet is based on data-mining the users of these services for targeted advertising. If you think the recent OPM hack revealed a lot of very private information, wait until the combined docket of your search, browsing, emailing, hangout-ing, social networking, and browsing preferences gets hacked.

I like to think of this in the frame of the saying; "If you want to go fast, go alone. if you want to go far, go together." Open Source is going together, and centralized services are going fast. They both serve valuable roles, and the history of technology is their interplay.

Dropbox is a fine example. The more geek set of us has been able to sync files across multiple devices on the network for quite some time, using a variety of technologies, from rsync to various version control systems, depending on the specific use case. It didn't always work, but if you were able to set it up, you were also able to debug it for the low low cost of a weekend spent inside. Dropbox took this need, unmet for the general populace, and made it Just Work, and work smoothly, with nice backup options, a universally available web interface, and clients that work across not just one or two OSes, but almost all of them, including mobile. That's pretty darned amazing, and it took not only vision but concentrated effort, design, and testing (which has a high cost). The trail they blazed has made it easier for a new round of open source alternatives to move towards normal-person-level usability (OwnCloud, SparkleShare), and even more decentralized options are on the horizon, with the closed-source work of BTSync and the open-source work of Tahoe-LAFS -- arguable both building off of the concepts first popularized by freenet and other p2p filesharing systems in the late 90s/early 2000s.

You can watch this happen in real time with chat right now. Skipping a really long dive into telegraphs, let's start with "talk" and "ytalk" - old server commands you could use to chat with other people logged in to the same server (this is from when you had to dial in or telnet over to a Unix or VMS server to check your email, predating this fancy web thing). This evolved into a shattered landscape of closed-source chat systems (ICQ, AIM, and many others), which meant you were often running 5 different chat apps just to keep in touch with all of your friends (not unlike the mobile landscape today, actually...). A few clients (Trillian, and later, Pidgen) evolved to be able to talk to multiple different services, and eventually an open standard emerged (XMPP) that big players adopted (gChat, Facebook chat). XMPP was fun, because anyone with an XMPP account could talk to anyone /else/ with an XMPP account, regardless of the "host" --- gchat users could talk with facebook users, or you could set up your own server even and have the same access. Now, gChat has locked out other users, Facebook is ditching XMPP support, and we're returning to a collection of walled gardens. Some of this is because the XMPP standard needs improvements, but it's also a type of rent-seeking by various social media networks to better capture their users -- good for advertising, bad for us.

<h3>Security, Federation/Decentralization, and the Risks</h3>

Adding security on top of this is complex - a funded company is able to hire network engineers and network security staff to both securely configure and actively monitor their systems -- but they're not "required" too, and there is rarely anything other than marketing statements on a website to offer "proof" that this is happening. The flip side is rarely better, though - an under- or un-funded project without dedicated net security staff tossing up a server (is it configured? hardened?) and hosting a collection of open source tools (have they been audited? is **anything** being updated??) is not any better -- and in my experience, is often much worse in practice.

Sustainability is hard, funding for core, quality, long-term security support is incredibly challenging, and the adversaries -- be they automated bots looking to insert ads in your website, annoying hackers who don't like you, or sophisticated and powerful actors -- are constantly improving.

<h3>Impact</h3>

A great challenge a colleague once asked me, on technology and international development, was this: Who has done more to connect people with life- and livelihood- saving information, and to connect the "bottom billion" -- 50 years of international development projects or the last decade of work by private, for-profit mobile phone providers? This was almost 10 years ago, when the world was going from an insignificant number of people with any connection, however tenuous, to the global Internet, to an astounding number connected via SMS and feature-phones.

In digital security today, I think there's a new valid question to ask. For the "normal" person - what has done more to increase their security and privacy - the past 5 years of Google's efforts, or the past two decades of open source tool development?

It's a hard question, and a mean one. I support - strongly, personally and professionally, the development of secure, open source tools to protect sensitive information and the incredibly people on the front lines of progress and protecting human rights. Google has been key in forcing increased adoption of secure connections (SSL, now TLS) - first across webmail providers and now among websites interested in preserving their search rankings. Through its Chrome browser, it's pushing sites to upgrade from older, less secure certificates, and providing a high level of security many key sites (until a better technology - HSTS - becomes more popular).

<h3>Conclusions</h3>

There's no actual real answer to this collection of challenges. At a base level, consider what you're actually worried about and choose your tools accordingly. I personally try to encourage the use of open source technologies, but not at the cost of not getting things done. Given the choice between a tool that is totally open, reviewed for security, and impossible to use, and one that is closed source, with a solid track record on security, and super easy to use - I'll likely suggest the second, with a short conversation about the benefits and risks in that decision. I'd prefer everyone to be more secure with tools they are comfortable using than to be confused and angry.

But this answer is shallow, and very dangerous in the longer term.  As a global community of technologists, geeks, makers, and do-ers, we need to push for open source tools, open standards, and work to make them both secure and usable, as centralized platforms all have a lifespan -- but let's not let the perfect be the enemy of the good, and while we rebuild a more decentralized architecture, let's adapt to what we have now as well.
