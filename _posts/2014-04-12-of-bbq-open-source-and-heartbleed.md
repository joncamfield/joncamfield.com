---
excerpt: "There's a point here about heartbleed and security — I promise."
categories:
- web 2.0 and f/loss
- hactivismo
- floss
tags:
- heartbleed

header:
  image: /assets/images/heartbleed.png
  teaser: /assets/images/heartbleed.png
  caption: "Heartbleed icon"

title: Of BBQ, Open Source, and Heartbleed.
created: 1397351518
---
There's a point here about heartbleed and security — I promise. Keep with me.

As I am wont to once the weather finally begins to coöperate, I've been trying a few new things out on the grill.  When I'm in this exploratory phase, I love digging through the infinitely interesting BBQ blogs of the Internet - they're full of hard-won knowledge about fire and smoke, but often lack a certain level of technical polish.

Case in point, my reference blog for this week's experiment was a well-seasoned old blog, but they'd lost every single comment from years of discussions. Why?  No technical glitch, but simply because they'd chosen a private company to manage their comments - and it went out of business, leaving them not only without a commenting tool, but without those years of educational clarifications and discussions.

Ownership and control matter.  This is true when you're talking about your possessions, your house, your comments on a BBQ blog, and with your software. I've railed <a href="//joncamfield.com/blog/2012/01/against_appification">against app-ification</a> before, but I want to make a slightly deeper point here.  If you bought a house, but with the condition that any repair, no matter how minor, you had to contract the previous owner (and only them) to make at a cost of their choosing - would you feel you really owned or controlled that house?  Would you buy a car where the hood was locked shut, accessible only to the specific dealership where you bought it?

These cases are very much the situation with the vast majority of software you run on your computer.  From Microsoft Word to Apple's iTunes, and even more insidiously, OSX and Microsoft Windows themselves - are all locked away from you.  You've been forced to pay hundreds of dollars for them with the purchase of any computer - but you have no control or real ownership over them.

<h2>Open Source</h2>
The alternative is what's called "free" or "open source" software (people get into fierce debates on the terminology here, which I'm ignoring for the time being).  All software starts with instructions that are more-or-less understandable by humans; commands like if (this thing) then (do this other thing).  Generally speaking, this "language" is then turned into something that's closer the more basic tools that computers understand. Imagine a particularly skilled dog with a great memory - by stringing together enough fetches, play deads, stops, roll overs and so on, you could eventually come up with a sequence of commands that would have this dog go out and buy a beer for you at the corner store, and bring in back.

"Closed source" software only gives you the computer-understandable version, and it's surprisingly difficult to turn that back into a simple, human-understandable chunk of logic.  "Open source" software, on the other hand, always provides you with the original, understandable language.

This means a lot of things - one, you can tweak it.  If you don't like the beer that your dog fetched, you can find the human-speak parts of the commands where it's selected, and make sure your preference for hoppy beer is respected, and then turn it back into the commands your computer can do.

This ability to change how your own tools work itself has many additional benefits - you can share that change, and if it's useful enough, that change itself will be included in the next version of the "core" software that everyone uses.

<h2>And finally, Heartbleed</h2>
This openness also means anyone can look at the logic that is driving their tool.  This means that when you start talking about trusting software, there's a heavy preference towards the software that you can look at the source code of, and even more preference towards software where a lot of people have been looking at this same code.

So, that failed with <a href="http://heartbleed.com/">heartbleed</a>.  The team behind OpenSSL is tiny compared to their impact.  Two out of every three secure servers in the world are running the software that this <a href="https://www.openssl.org/about/">four-person team</a> manages.  And on New Years Eve 2011, one of their developers committed a very, very subtle piece of code that basically didn't make sure that all the doors were closed behind it, and no one else at the time (or anyone who'd taken a look the in two years and chance since) noticed.

So obviously the whole open source thing is broken, right?  The bug is out in the open for anyone to figure out, but no one fixed it!

It's not quite so simple.  Do you really think that a working piece of closed-source code gets a second glance by its development team?  They're just as bound by priorities and shipping product releases as an open-source team, but their code gets locked away with not even the chance for a third party to find a bug and lend a hand — but it's no more secure than the open source tools from concentrated probing, and testing for flaws just like heartbleed.

So yes, heartbleed was bad, but it was also a reminder in how powerful the open source software world can be in finding and fixing a bug.  Most of us woke up with some updates to install, and that was the end of it.  What horrible, dark bugs are lurking, unfindable, in every piece of closed source software?  The precise number is unknowable, but the prevalence of viruses and malware that affect deeply closed systems like Windows might be a strong hint.

<h2>No more broken hearts</h2>
Going forward, I obviously have a long wishlist of things I'd like to see - a public discussion on what trust in software really means, better tools on every platform to guarantee software packages are what they claim to be (Tor is doing <a href="https://blog.torproject.org/category/tags/deterministic-builds">amazing work</a> here), a return to inter-operable standards, especially when we're talking security systems... But as a beginning point, simply better support structures for open code development would be nice. We have volunteers building the basic structures of the Internet - which is an absolutely amazing and good thing - but let's make sure they have the time and resources to do it.
<!--break-->
