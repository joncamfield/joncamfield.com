---
excerpt: "What security and safety tooling do we need to build now if Mastodon scales to tens or hundereds of millions of users."
categories:
- human rights
- web 2.0 and f/loss
header:
    overlay_image: /assets/images/0756_ManaPools_ZM_IMG_09354.JPG
    overlay_filter: 0.5
    teaser: /assets/images/0756_ManaPools_ZM_IMG_09354.JPG
    caption: "Elephant with Tusks at Mana Pools; CC-BY-NC-SA Jon Camfield"
title: From the Tusks and Safety Department
created: 2022-11-09
---

Even a moderately successful Mastodon fediverse will face a growing tide of increasingly annoying, dedicated, and scaled threats. This is not to encourage hand-wringing and giving up, but to start thinking about the next few months and years -- and what types of communities, processes, and systems we need to start building now.

Exclusionary hatespeech can (and does) fester on its own servers, but we have no responsibility to help it spread across the rest of the fediverse. I wrote about this [last year](https://www.joncamfield.com/blog/2021.05/centering-decentralization), but it will be critical, immediately, to stand together (and listen to!) with victims of harassment as Mastodon scales. Failing to do that might not immediately impact the cis-white-techy-early-adopter culture, but it will eat at the community and kill it off sooner than you might think. This is hard, and early adopters like myself (see above) will need to face some bitter truths relatively quickly and repsectfully.

## The usual suspects

Griefers, trolls, hatespeech, and personal attacks will build. They are already and will continue to disproportionatly target women, BIPOC, LGBTQIA+, and marginalized communities in the fediverse as elsewhere. I've seen a variety of advice basically saying "block early, block often" -- and I think that's great. Let us all -- as users and admins -- start fresh, in allyship, and with a clear signal that we're not here to deal with bullshit. Mastodon has a better starting position as a platform with built in moderation tools, ways to export and import block lists at the user and server level, content warnings and (overly complex) post privacy settings show an amazing amount of thought baked in, which will serve the growing community well.

...but this itself won't be enough.

Mastodon does not have a seasoned, scaled, round-the-clock, multilingual content moderation team.  Each server has its singular admin and maybe some (likely volunteer) moderators.  **Without diverse voices, Mastodon will not thrive.** We are going to have to adapt to leveraging the tools Mastodon does have, but in ways that don't continue to alienate communities.  I think there is a path through here, but it is going to take people doing moderation work to be careful, and educate themselves on some sharp corners of our world.

On top of that, we're already starting to see a few community divides on policy issues around who to allow in, and what servers have done de-federating-level offenses in increasingly fuzzy areas. I think these are to be expected, and will point the way to some visualizations and features help users and administrators understand what federation looks like.

## Same song, second verse - could get better, but...

As trolling gets worse, it will tax server admins, driving increased needs for support strategies for them to manage disputes and build up moderation support.

At the same time, relatively boring but impactful attacks will probably start targeting instances -- from just griefers to people angry at instances for blocking their server, objections to policy calls, and so on. These will be DDoS attacks of varying levels, as well as targeting well-trodden vulnerabilities. Skilled server admins already have some good tools to deal with this, but it will add another layer of noise, cost, and complexity for admins.

Both of these will reduce hobbyist hosts (like myself) and cause some level of centralization in larger, more resourced instances -- though it would be great to see tool suites built up to help defensive work on this continue to scale to the entire server host community.

## Federated, scaled, and rapid response: Choose 1

Incentivized adversaries will get beyond where user and instance blocking is sufficient if there's value in doing so.

The fediverse needs to start building processes and systems for semi-automated threat information sharing and management, and find ways to build it to thrive in a closed community among trusted server admins, with a process to feed it out, openly, to all admins. This system will provide the speed and trust to tamp down malicious actors while also building a high-trust community which can also respond to future emergent attacks. (Yes, this is something I've been [hammering on](https://www.joncamfield.com/blog/2021.05/centering-decentralization) for human rights tech for [a while](https://www.joncamfield.com/blog/2019.02/cyberpunk-standards.html).)

## But now we get to the other hard parts.

First, consensus on complex policy calls on emergent, rapidly-evolving problems will be hard. Sure, each instance can decide independently, but this further squeezes small and medium sized instances. The best option will be information and policy sharing among instances, but openly dealing with subtle operations by well-resourced adversaries — at scale and across instances — is going to be ROUGH. We're not even talking nation-state actors, merely dedicated scammers/spammers.

Looking further forward, the Mastodon fediverse will need to figure out how to deal with user-data requests, subpoenas, and all sorts of challenges which can directly impact the livelihoods of server admins as well as the code contributor community. These will come from all sorts of places, and make the open policy consensus and threat information sharing problems vastly more complex.

Both democracies and authoritarian states around the world have made it clear that they will straight up imprison people who are refusing access to data, good faith code contributors, as well as try to implant bad faith ones to get their way. This will impact where admins can live and where they can travel. It impacts where they host their servers, and whose code they accept. Again, there are some ways to minimize impacts on this for most users/servers -- from moving to reproducible builds and really tight code to app security processes, log minimization, regular public security audits, and maybe (while drawing in its own risks) somehow adding e2ee for DMs to simply erase what data a server admin has access to that isn't public. But again, this also adds steep further requirements onto instance hosts.

All of this is not to be discouraging, but to think about what we need for this crazy experiment to work, and to scale enough to keep working. We all [deserve it](https://www.joncamfield.com/blog/2022.11/on-mastodon.html).

### Some links and resources that inspired this

* This amazing thread popped up as I was finalizing this post [@schock@mastodon.lol](https://mastodon.social/@schock@mastodon.lol/109384005025090282)
* [@jerry@infosec.exchange](https://infosec.exchange/@jerry/109296684462206872)
* [@dyn@infosec.exchange](https://infosec.exchange/@dyn/109291211783459825)
* [TechDirt: Gab, Mastodon And The Challenges Of Content Moderation On A More Distributed Social Network](https://www.techdirt.com/2019/07/16/gab-mastodon-challenges-content-moderation-more-distributed-social-network/)
* [Surviving the Fediverse on a Mastodon](https://treacherous.tech/mastodon.html)
* [TechDirt: Hey Elon: Let Me Help You Speed Run The Content Moderation Learning Curve](https://www.techdirt.com/2022/11/02/hey-elon-let-me-help-you-speed-run-the-content-moderation-learning-curve/)
* And finally I cover a lot of this at an even less pragmatic level in [Centering Decentralization](https://www.joncamfield.com/blog/2021.05/centering-decentralization).
