
* local laws - compliance or... ? (e.g. laws prohibiting encrypted comms)

* security as an afterthought (voting app story; only an afterthought until it burns you... at least for a few rounds after that...)
* Reminiscent of HCD as a bolt-on?

## Intro 

I'm Jon Camfield, senior technologist at Internews. I work across our digital portfolios, directing projects creating a framework for security audits built for NGOs, creating more usable security tools, and also advancing the leading edge of privacy and security tool capabilities. I also lead the digital components of an organizational-wide operational security team.
 
## What-Ifs on Cuban Twitter :10 (→2:40_)

**ACTIVITY** What was wrong about Cuban Twitter?? (Write up topics as students propose them)

	Backups:

* Beneficiary-led needs
* Informed consent
* Unclear understanding of Cuba's capabilities
* Dubious acquisition of phone numbers
* Lack of policies around privacy and data gathering

**Activity** What did the project do /right/ ?

	Backups

* USAID realized the project's USG backing was problematic
* Indirect connections, "obfuscation" of source servers
* Operating like a social media startup
* Reigned in "push" messaging

What ifs:

* What if Zunzuneo had purely been a peer-to-peer messaging system, with no intention of political messaging meddling?
* ...based on user demand/needs?
* What if it still had gotten leaked, and people with dissident comments or even merely quotidian frustration were put at risk?
* What if it happened in a country where the government regularly not just arrested, but also tortured activists?

Linda Raftree covers the ethical questions around this work really well. If I could sum it up in one catch-phrase, it would be to always monitor who is driving the project - beneficiaries, or funders?  I can guarantee that that becomes a very muddy distinction very quickly.

It's easy to start down a long path of discussion on the role of development global politics, but that's not what I want to get in to today, unless Wayan has a whiskey budget.

## Not Isolated Cases :15 (→2:55)

It doesn't take a quasi-covert democracy program to get into dangerous waters in security and privacy (they do make for great case studies though).

I want to focus our discussion today on privacy and security aspects that touch every single ICT4D project:

* Informed consent
* Risks
* Mitigations

**ACTIVITY** What areas of development do you find most interesting? (Write up topics as students propose them)

A lot of development work is going to run into people who oppose it, or people who are resentful or scared, or it simply will upset a power structure.

(Walk through quick case studies based on interested topics)

* Journalism/Media development - Reporta app http://motherboard.vice.com/read/this-new-secure-app-for-journalists-may-not-be-secure-at-all
* Human rights documentation - ISIS story http://www.nbcnews.com/storyline/isis-terror/raqqa-being-slaughtered-silently-activist-killed-urfa-activist-group-says-n454386?cid=sm_tw&hootPostID=7fe7537da5bbbab6c757015fa5525764 
* Election monitoring - Uganda https://www.privacyinternational.org/node/656 
* Also... LGBTI rights
* Education - girls' education in particular
* ICT4Health ...

Example with health care:

	Let's talk health care tracking apps via mobile and SMS.  Who automatically has access to that data? How protected is it?  What would happen if it leaked? Does anyone /want/ it to leak? 

	We still need to keep information security in mind. No one wants their medical history, prescription data, drug adherence, or HIV status leaked and made public - but the number of ICT4D interventions that transmit this over SMS to be stored on some aid worker's laptop as an excel file is mind-boggling.


## Adversaries :10 (→3:05)

I want to move on to a few exercises I find to be useful in understanding risk, but we also have to talk about **practicality**.  This has been the biggest piece we've focused on in our SAFETAG audit framework for NGOs -- giving a laundry list of everything that could possibly go horribly wrong is defeating, and does not result in any change.  

In addressing risk, we have to add in the impact as well as the likelihood, and for that we need to consider the potential **adversaries**, and their capabilities and motivation.

### Global Baseline Risks (→3:05)

This is a highly contentious discussion, but I'm a strong believer in the ability to agree on a baseline level of risk and collection of adversaries that you must be capable of defending against.

* Scams and phishing - you are not a unique and valuable candidate to help anyone get millions of dollars out of anywhere
* Boring Adware / malware - automated hacks, CMSes, search toolbars
* The laptop at the airport
* The leak to the media
* The Angry Ex Employee / Disgruntled Employee

Most of these are easy to mitigate! (whiteboard these)

* Updated (and legal/licensed) software
* Updating Anti-malware/anti-virus tools
* Encrypted hard drives and travel procedures (VPNs!)
* Not running as an admin user
* Strong passwords
* Enforced data management policies (need-to-know access) (this gets hard!)

### Break for questions?

* Servers, clouds, SaaS, oh my!

### The Real-life bad guys (→3:05)

The good news is that the mitigations for these also make more targeted attacks by real-life adversaries much less likely to succeed!

It's hard to find a country in the world that hasn't enacted legislation and/or purchased surveillance and malware tools to prey on its population.  This used to be China, Russia, Iran and a small handful of others; but surveillance has gone commercial.

* FinFisher, HackingTeam
* Govt-back spearphishing, customized and targeted malware
* infiltrating / abusing networks of trust (digital rapid response)

[screenshots of tech support from finfisher?]

It's worth doing even just a few hours of research on the threat landscape of any country you're looking to work in, and to update that when you travel there yourself.  USG funders are beginning to expect risk analyses with proposals and clear plans for mitigation.  This is a great thing, and the time is now to get out in front of this.

-------------------------

## Risk Modeling 101 :20 (→3:25)

When I work with orgs and consult on projects, I find a few core activities to be really useful to think through the critical points to really think about what is happening and where the potential failure points are ; then moving to what the impacts would be, and finally focusing in on likelihood

**Activity** Process Mapping: Coursework

**Activity** Data Mapping: (Project?)

* Patricia: where does the data sit, and who owns it?  (servers at MO???, cloud hosting, +govt partners?? )

**Activity** Action movie risk identification with the CIA

Let's first cover a classic chunk of information security.  One of the worst parts about infosec is that we've found innovative new ways to use synonyms to mean completely different things.  In the lingo, a vulnerability is not a threat is not a risk.  But we do have some approachable core concepts that are useful to frame discussion using:

CIA Triad: Confidentiality, Integrity, Availability 
	https://en.wikipedia.org/wiki/Information_security

If you want 10 opinions on infosec, ask 5 experts - additional principles that flesh these core concepts out to over 30 different specific items.

## Wrap up / Qs / Resources :5 (→3:30)

What if this data had been even remotely sensitive? (return to case study walkthroughs)

Resources:

* TTC / SIAB
* SAFETAG.org , safetag's resource sections
* DFAK
* https://www.theengineroom.org/new-staff-security-checklist/


--------------
**Activity** Bow-tie security ("action movie")


RAFT:

	(30 mins) Process enumeration activity (from SAFETAG)

	(30 mins) Critical Data Activity + Data sensitivity (matching data to processes) (from LevelUp and SAFETAG, lightly modified)

	(30 mins) Identifying risks - walking through the processes and asking what all could go wrong (modified "Action movie" approach); using CIIA (Confidentiality, Integrity, Identity, Accessibility)


## Scary World Out There


What is everything that could be a problem for a health monitoring program with ICT components? (write up ideas, loosely organized around a likely core data breach - loss of a laptop, 

Let's look at one lonely one - 

What could have caused this?  What could this cause?





----------
## Let's apply the CIA to election monitoring.

* Confidentiality: While eventually public, live data and per-election-monitoring staff can need to be confidential to prevent violence
* Integrity: Only election monitors should be able to provide data, and the data they provide shouldn't be able to be changed; The monitoring agency has to know who the monitors are, but it may put them at risk to be publicly known
* Availability: Monitors have to be able to access the monitoring system to provide updates, and the results of that system have to be publicly accessible

## But Why?

That may have seemed easy.  It's because we skipped an actually important step.  We never defined our environment.

## Risk Modeling

Hypothetical story about election monitoring. This absolutely has never ever happened at all to me.

Organization washes up on my email doorstep.  They've been building an android app from scratch (of course) to collect election data.  The election in the country they're operating in has been called, and they're ready to go, but want to know if there are any security steps they should make, as the government does not want the elections monitored, and they're worried about harassment or imprisonment of anyone doing so in a coordinated fashion. 2 weeks to election day - go!

**Activity** What would you recommend?


-------------------------------

## Week 10: November 2, 2015 Principle 8: Address Privacy and Security

* Assess and mitigate risks to the security of users and their data. 
* Consider the context and needs for privacy of personally identifiable information when  designing solutions and mitigate accordingly. 
* Ensure equity and fairness in co-creation, and protect the best interests of the end-users. 

This session will explore privacy, security, ethical considerations, and regulatory issues that  affect human rights in a way that either stimulates or impedes innovation. Students will be asked  to determine what types of ethical issues and regulatory constraints may have an impact on their proposed projects and to make recommendations on how they might overcome such hurdles.  The session will also look at the role technology is playing in financial inclusion. 

Required readings:

Haikin, Matt (2015). If Digital Freedom is a Myth, How Can We Ethically Provide Access to  Cutting-Edge Technology? Available from: http://www.ictworks.org/2015/02/18/if-digital-freedom-is-a-myth-how-can-we-ethically-provide-access-to-cutting-edge-technology/

Hege, Asia (2015). Tweet Tweet! Cuban Twitter and its Implications for ICT4D. Available from:  http://technologysalon.org/tweet-tweet-cuban-twitter-implications-ict4d/

Maisonet-Guzman, Olimar (2015). Gender-Violence 2.0: The Digital Safety Gap for Women.  Available at: http://www.ictworks.org/2015/01/12/gender-violence-2-0-the-digital-safety-gap-for-
women/

Phelps, Denise (2015). 5 Unanswered Questions on Expanding Digital Economies in Developing Countries. Available from: http://www.ictworks.org/2015/05/11/5-unanswered-questions-on-expanding-digital-economies-in-developing-countries/

Raftree, Linda (2014). Zunzuneo and ethics in technology for democracy. Available from: http://lindaraftree.com/2014/05/06/zunzuneo-and-ethics-in-technology-for-democracy/

Shamas, Norman (2014)Responsible Development Data - Practitioner's Guide. Available from:  https://github.com/tanialee15/Responsible-Development-Data

Trust Law Connect & mHealth Alliance (2013) Patient Privacy in a Mobile World: A framework addresses privacy law issues in mobile health. London: Trust Law Connect. Washington, DC:  mHealth Alliance.

Vota, Wayan (2014). Dear USAID, What Were You Thinking with Cuban Twitter? Available from: http://www.ictworks.org/2014/04/04/dear-usaid-what-were-you-thinking-with-cuban-twitter/

Vota, Wayan (2015). The Number One Reason You Do Not Encrypt Email. Available from:  http://www.ictworks.org/2015/05/22/the-number-1-reason-why-you-do-not-encrypt-email/

Recommended resources: 

http://digitalprinciples.org/address-privacy-security/

http://betterthancash.org/resources/publications/

http://pdf.usaid.gov/pdf_docs/PNADN040.pdf

http://www.ictworks.org/2015/06/03/new-usaid-toolkit-how-implement-electronic-payments-in-development-programs/

Case Study: Digital Financial Services


