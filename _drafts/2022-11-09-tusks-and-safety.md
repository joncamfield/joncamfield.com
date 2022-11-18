---
excerpt: "What security and safety tooling do we need to build now if Mastodon scales into tens or hundereds of millions of users."
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

I want to map out the threats that even a moderately successful Mastodon fediverse will face, going beyond my [rose-colored-glasses version](https://www.joncamfield.com/blog/2022.11/on-mastodon.html) . This is not to encourage hand-wringing and giving up, but to start thinking about the next few years and what types of communities, processes, tools, and systems we need to start building now.

What follows is a quick thought exercise of what attacks we should expect if Mastodon stays on this trajectory and scales into millions of users.

## The usual suspects

Griefers, trolls, hatespeech, and personal attacks will probably be manageable-ish for a while, and target women, BIPOC, LGBTQIA+, and marginalized communities in the fediverse as elsewhere. I've seen a variety of advice basically saying "block early, block often" -- and I think that's great. Let us all -- as users and admins -- start fresh, in allyship, and with a clear signal that we're not here to deal with bullshit.

Exclusionary hatespeech can fester on its own servers, and we have no responsibility to allow or help it spread across the rest of the fediverse. I wrote about this [at length last year](https://www.joncamfield.com/blog/2021.05/centering-decentralization), but it will be critical, immediately, to stand together with victims of harassment as Mastodon scales. Failing to do that might not immediately impact the cis-white-techy-early-adopter culture, but it will eat at the community and kill it off sooner than you might think.

## Same song, second verse - could get better, but...

As trolling scales, it will tax server admins, causing either a reduction in mid-sized and large open servers, or a push/requirement for some funding or support/service strategy for them to manage disputes.

Varieties of DDoS attacks, from just griefers to people angry at instances for blocking their server, objections to policy calls, and so on, will also happen. We have some good tools to deal with this, but it will add another layer of cost and complexity for admins.

It's worth noting also that incentivized adversaries will get beyond where user and instance blocking is sufficient if there's value in doing so.

That said, it is good to see already active server-block-list coordination and the beginning of more automation for admins. That will get both vital and complicated, as more diverse server admins choose to allow/disallow more nuanced annoyances.

## Federated, scaled, and rapid response: Choose 1

Consensus on complex policy calls on emergent, rapidly-evolving problems will be hard. Sure, each instance can decide independently, but with many having a staff of 1 volunteer each, that is unrealistic. Adversarial dodging of whatever gets decided in the open will be easier.

Similarly, openly dealing with subtle operations by well-resourced adversaries — at scale and across instances — is going to be ROUGH. We're not even talking nation-state actors, merely dedicated scammers/spammers.

In my opinion, the system we should start building ASAP is a group of processes for semi-automated threat information sharing and management, and find ways to build it to thrive in a closed community among trusted server admins, with a process to feed it out, openly, to all admins. This system will provide the speed and trust to tamp down malicious actors while also building a high-trust community which can also respond to future emergent attacks.

## And now we get to the hard parts.

Looking further forward, the Mastodon fediverse will need to figure out how to deal with user-data requests, subpoenas, and all sorts of challenges which can directly impact the livelihoods of server admins as well as the code contributor community.

Both democracies and authoritarian states around the world have made it clear that they will straight up imprison people who are refusing access to data and good faith code contributors, as well as try to implant bad faith ones to get their way.

This impacts where admins can live, where they can travel, and where they host their metal. There are some ways to minimize impacts on this for most users/servers -- from moving to reproducible builds and really tight code to app security processes, log minimization, regular public security audits, and  somehow adding e2ee for DMs to simply erase what data a server admin has access to that isn't public.


## Let me conclude with a few pointers for further reading:

* [@jerry@infosec.exchange](https://infosec.exchange/@jerry/109296684462206872)
* [@dyn@infosec.exchange](https://infosec.exchange/@dyn/109291211783459825)
* [TechDirt: Gab, Mastodon And The Challenges Of Content Moderation On A More Distributed Social Network](https://www.techdirt.com/2019/07/16/gab-mastodon-challenges-content-moderation-more-distributed-social-network/)
* [TechDirt: Hey Elon: Let Me Help You Speed Run The Content Moderation Learning Curve](https://www.techdirt.com/2022/11/02/hey-elon-let-me-help-you-speed-run-the-content-moderation-learning-curve/)
* And finally I cover a lot of this at an even less pragmatic level in [Centering Decentralization](https://www.joncamfield.com/blog/2021.05/centering-decentralization).
