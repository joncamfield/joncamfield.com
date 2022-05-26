---
excerpt: "Let's rewind back to the 90s.  Denial of service was a very, very different thing then"
categories:
- development theory
- networks
- human rights
- ict policy
tags:
- deflect
- ddos
- floodnet

header:
  overlay_image: /assets/images/FloodNet300.jpg
  overlay_filter: 0.5
  teaser: /assets/images/FloodNet300.jpg
  caption: "Floodnet screenshot"

title: Distributed Solutions for Distributed Attacks
created: 1382395841
---
Google has been making headlines with their shiny <a href="https://projectshield.withgoogle.com/about/" target="_blank">Project Shield</a> which wraps PageSpeed with other tools to defend sites against denial of service attacks. The history of the denial of service, however, runs deep, and underlines that no centralized response to it will ever be able to cost-effectively scale against a distributed attack.

Let's rewind back to the 90s.  Denial of service was a very, very different thing then - it was a tool <strong>for</strong> free expression, not one used to mute dissenting opinions as it is today.
In the dot-com boomtimes of the late 90s, I was absolutely fascinated by the digital protests that sprung up in reaction to Mexico's treatment of the Zapatista Movement.  <a href="https://www.thing.net/~rdom/ecd/ZapTact.html" target="_blank">Floodnet</a> was an activist art project by the <a href="https://en.wikipedia.org/wiki/Electronic_Disturbance_Theater" target="_blank">Electronic Disturbance Theater</a>.  Floodnet was simply a website you could visit and it would direct your browser to constantly reload pages on the website of the Mexcian government.  In addition to overloading the website with thousands of requests from you and our fellow programmers, you could add in a political message with each page load, to force the government's server to fill their log files with messages like "human rights not found."

<blockquote style="float: left; text-wrap: normal; width: 55%">"The FloodNet application of error log spamming is conceptual Internet art. This is your chance to voice your political concerns on a targeted server. [...] The server may respond to your intentional mistake with a message like: "human_rights not found on this server." So by creatively selecting phases, you can make the server voice your concerns. It may not use the kind of resources that the constant reloading uses (FloodNet automatically does that too), but it is sassy conceptualism and it invites you to play with clever statements while the background applet is running." (via https://www.thing.net/~rdom/ecd/ZapTact.html) </blockquote> <div style="float: right; width: 305px;"><a href="https://www.thing.net/~rdom/ecd/ZapTact.html" target="_blank"><img src="/assets/images/FloodNet300.jpg" align="right" border="0" hspace="2" alt="Floodnet used DoS attacks to protest the Mexican Government"></a><br /><span class="caption" style="color: #444;">Floodnet used DoS attacks to protest the Mexican Government</span></div>  <br clear="left" />

This original "denial of service" attack was seen as the digital mirror of a classic "sit-in" protest. It was a way for a David to strike back at a Goliath through technology.  However, this, ahem, "sassy" political activism began an arms race that today is dominated by Goliaths alone.  Instead of a tool of protest, denial of service attacks are today tools of retribution and ways to mute dissenting voices.  They are massively automated and distributed, and are run not by rowdy bands of dissidents, but by well-organized for-hire groups (https://krebsonsecurity.com/2013/05/ragebooter-legit-ddos-service-or-fed-backdoor/) and even from government infrastructures.

The only defense, so far, has been equally massive, and centralized, commercial services. This is a growing industry with its <a href="https://www.fastcompany.com/3008201/code-war/ddos-protection-squad" target="_blank">own round of disruptive innovators</a> all to itself.  This current business innovation is helping to move from the monolithic services protecting online infrastructures at high costs to a more scalable model, with services that smaller websites can benefit from. Still, back-end models are the same - providing shelter from DDoS attacks by having sufficient servers and bandwidth to absorb whatever their proprietary tools and filters cannot outright block.

Open source models to fight back have been conspicuous in their absence - until now.

<a href="https://deflect.ca/" target="_blank"><img src="/assets/images/deflectlogo_RED_small2.png" border="0" align="left"  hspace="5" /></a> <a href="https://deflect.ca/" target="_blank">The Deflect Project</a>, created by the eQualit.ie technology collective based out of Montreal and Dublin, is responding to that gap.  They focus on providing protection for activists and journalists around the world, who are subject to DDoS attacks from those who disagree with their views all the way to their own governments.  Thanks to grant funding, Deflect is able to offer their services for free to independent media sites, NGOs and non-profits -- but the technology model under the hood is the real game-changer.
<!--break-->
Deflect, first and foremost, is open source.  It's built to run on a network of low-cost virtual servers, meaning anyone could spin up a DDoS-resilient network and support their own cluster of sites for a very manageable (and scalable) ongoing cost.  Deflect does this by building efficient deployment and management tools on top of popular and well-supported open source projects, and adding new features where they've found the field lacking.  The group is currently evolving a fully open-source machine-learning system which can autonomously detect and respond to dynamic attacks.

The next step, currently under active development, is an even further distributed style of Deflect, where anyone can offer a bit of their server and bandwidth capacity to help out an instance of Deflect, including even the beneficiaries themselves; helping out others in their network who are being DDoSed while they themselves are not.  The collective plans to take this concept of openness further still.  As this distributed network comes online, the system will also enable independent Deflect networks and volunteer nodes to share botnet patterns they have gathered with the broader Deflect community.

This, in a way, is fighting fire with fire -- but it's more than that.   Deflect at is core is building a system to provide collaborative support around reacting to a challenge.  Not unlike, actually, FloodNet.
