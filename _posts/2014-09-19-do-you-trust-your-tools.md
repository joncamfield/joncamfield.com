---
excerpt: "Let's actually talk about how you might
  have trust in a software project, using Tor as an example."
categories:
- web 2.0 and f/loss
- hactivismo
- human rights
- tor
header:
  overlay_image: /assets/images/ashim-d-silva-Kw_zQBAChws-unsplash.jpg
  overlay_filter: rgba(0, 0, 0, 0.5)
  teaser: /assets/images/ashim-d-silva-Kw_zQBAChws-unsplash.jpg
  caption: "Photo CC0 Ashim D Silva / Unsplash"

title: Do you trust your tools?
created: 1411135501
---
There's a budding conversation on <a href="https://twitter.com/Dymaxion/status/512833189715259392" target="_blank">"trust" over in the twitterverse</a>.  I began a draft post a while back that compared <a href="https://www.torproject.org/" target="_blank">Tor (the amazing privacy and anti-censorship network</a> and all privacy-protecting software to condoms.  More on that soon, but let's actually talk about how you might have trust in a software project, using Tor as an example. Tor has been in the news recently, and I've had a ton of people ask me about how safe it is to use, so I figured one click-bait headline is as good as another in having an open and honest discussion about Tor.

First, let's be transparent.  Tor - not unlike <a href="https://en.wikipedia.org/wiki/History_of_the_Internet" target="_blank">the Internet itself</a> - did in fact start out as a project by the <a href="https://www.onion-router.net/" target="_blank">US Naval Research Laboratory</a>, and does continue to receive funding by the US Government to support freedom of expression around the world, with targeted efforts to enable free speech and access to uncensored information in countries where Internet connections are heavily filtered.

So, can you trust Tor?  How do you know that the NSA hasn't forced Tor into building a "back door" into the Tor software, like they did with <a href="https://www.theverge.com/2013/12/20/5231006/nsa-paid-10-million-for-a-back-door-into-rsa-encryption-according-to" target="_blank">RSA Security</a>, and <a href="https://www.theguardian.com/world/2013/jul/11/microsoft-nsa-collaboration-user-data" target="_blank">many other pieces of software you use daily</a>, or like what has historically happened to privacy-protecting services like <a href="https://www.wired.com/2007/11/encrypted-e-mai/" target="_blank">hushmail</a>?

The answer is actually that you should not actually need to trust the organization behind Tor in order to be confident that the software is built to be safe.  This is enabled by the fact that Tor is open source - meaning you can read every line of the code they use to build the software you install.  Of course, even with open source software, you're trusting whoever is compiling it do do so on a secure system and without any extra malicious intent.  The Tor Project answers this problem by using "<a href="https://blog.torproject.org/blog/deterministic-builds-part-one-cyberwar-and-global-compromise" target="_blank">deterministic builds</a>", which let you check, independently, that the code posted publicly is the code you're running.

If you use Windows or Mac, both "closed source" operating systems, you are absolutely, 100% trusting that no one in the company, nor any government with significant sway over these companies, has snuck in code to allow remote spying. You have no way to inspect the code running your operating system, and every tool you use on top of it is vulnerable to being undermined by something as simple as a hack to the tiny piece of software that tells your computer how to talk with the keyboard, which could just as easily also store every password you have ever typed in.  You're also trusting your ISP, every web site you log in to, and thousands of other intermediaries and companies, from the ones who provide SSL Certificates (enabling the "green lock" of a secure website) to the manufacturer or your wifi router and cablemodem to not betray your trust by accident, under duress, or with malicious intent.

Of course, even back in the green pastures of open source, there is no "absolute" level of trust, no matter how much we'd like there to be.  Rare is the user who actually checks the "signature" of the download file against the posted "signature" online to make sure the tool they're about to install is the intended one. And even rarer is the user who checks in on the deterministic build process (and it's still fragile, so hard to guarantee even so).  Even at this level, you are trusting the developers and others in the open source and security community to write solid code and check on it for bugs.  The Tor Project does an exceptional job at this, but as <a href="https://joncamfield.com/blog/2014.04/of_bbq_open_source_and_heartbl">heartbleed</a> reminds us, huge, horrible bugs can go unseen, even in the open, for a long time.  You're also trusting all the systems that the developers work on to not be compromised, and to be running code that is also in more or less good condition, and to be using compilers that aren't doing funny things.
For what it's worth, <a href="https://cm.bell-labs.com/who/ken/trust.html" tarhget="_blank">this is hardly a new problem</a>.  In my unhumble opinion, I'd still rather have this more open model of shared trust in the open source world than rely on any single company, whose prime motive is to ship software features on time.

So - can you trust Tor?  I do.  But saying that I "trust" Tor doesn't mean I have 100% faith that their software is bulletproof.  All software has bugs, and particularly security software requires a lot of work on the part of the user to actually make it all work out as expected.  It's time to talk about trust less as a binary and more as a pragmatic approach to decision making based on best practices, source availability, and organizational transparency.
<!--break-->
