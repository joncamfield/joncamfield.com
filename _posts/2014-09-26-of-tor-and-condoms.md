---
excerpt: "I am far from the first to compare digital security practices to safer sex
  practices; Jillian York even rapped about it on stage at re:publica in 2014"
categories:
- web 2.0 and f/loss
- hactivismo
- human rights
tags:
- tor

header:
  overlay_image: /assets/images/galriccondom.jpg
  teaser: /assets/images/galriccondom.jpg
  #caption: "Garlic flavored condom wrapper"


title: Of Tor and Condoms
created: 1411760350
---
I am far from the first to compare digital security practices to safer sex practices; Jillian York even rapped about it on stage at re:publica in 2014 (direct link removed as the video also includes a known abuser). <!--Heck, you can even see a rap career blooming as <a href="https://twitter.com/jilliancyork">Jillian York</a> and <a href="https://twitter.com/ioerror">Jacob Appelbaum</a> suggest that it's time that we <a href="https://www.youtube.com/watch?v=BBgZyV4iltw">"talk about P-G-P" at re:publica</a>.-->

<figure>
    <a href="/assets/images/galriccondom.jpg"><img src="/assets/images/galriccondom.jpg"></a>
    <figcaption>A garlic-flavored condom?</figcaption>
</figure>


A quick disclaimer: First, apologies for the at-times male and/or heteronormative point of view; I'd welcome more inclusive language, especially around the HTTPS section. Second, I am unabashedly pro-Tor, a user of the tor network, and am even lucky enough to get to collaborate with them on occasion. The garlic condom photo comes from <a href="http://thestinkingrosestore.com/display.aspx?catid=23,33&pid=2201" target="_blank" border="0">The Stinking Rose.</a>.

<h3>Super-duper Unsafe Surfing</h3>
Using the Internet without any protection is a very bad idea. The SANS Institute's <a href="https://isc.sans.edu/survivaltime.html">Internet Storm Center tracks "survival time"</a> - the time a completely unprotected computer facing the raw Internet can survive before becoming compromised by a virus - in minutes.  Not days, not even hours. This is so off the charts, that with a safer sex metaphor, using no protection is more akin to just injecting yourself with an STD than engaging in a risky behavior.

<h3>Barely less unsafe surfing</h3>
Adding in a constantly-updated anti-virus tool, and a firewall, and making sure that your operating system is up to date is akin to being healthy.  You have a basically operational immune system - congrats!.  You'll be fine if the person you're sleeping with has the common cold, but anything more serious than that and you're in trouble.

Using HTTPS  - visiting websites which show up with a green lock icon - is also a good practice.  You can even install some browser plugins like <a href="https://www.eff.org/https-everywhere" target="_blank">HTTPS Everywhere</a> and CertPatrol that help you out.

HTTPS is kind of like birth control.  You may successfully prevent *ahem* the unauthorized spread of your information, but you're still relying on a significant amount of trust in your partner (to have taken the pill, to withdraw), and there are things out of your knowledge that can go wrong - the pharmacist provided fake pills, or you have a withdrawal failure (please note this is about digital security advice, and not at all giving good safer sex advice - a quick visit to <a href="https://en.wikipedia.org/wiki/Comparison_of_birth_control_methods">wikipedia</a> is a good start for effective -- and non effective birth control methods!). With SSL Certificates, you are still trusting that the website has good practices to protect your information (insert the constant litany of password reset links you've had to deal with this year here), and there have been cases of <a href="http://www.wired.com/2011/08/diginotar-breach/" target="_blank">stolen SSL certificates</a>) and are tools to help an attacker <a href="http://www.thoughtcrime.org/software/sslstrip/" target="_blank">try and intercept your encrypted traffic</a>.

<h3>Slightly Safer Surfing</h3>
With digital security, a lot like with safer sex, some methods can be combined for a greater effect, but layering other methods can be a horrible idea.  Adding using anti-virus tools, firewalls, system updates, and HTTPS on top of any other method here is a universally Good Thing.

Using a VPN is like using a condom, provided by your partner for this encounter, and given to them by a source neither of you have any real trust in.  Asking the manufacturer for information about exactly how it's made, or what its expiration date is will often result in  grand claims (but no hard evidence).  Requests to see the factory floor and verify these claims are presumed to be jokes.  The VPN-brand condom generally works, and is definitely fast and easy, but you're placing a lot of trust in a random company you found while searching the Internet, and probably also the cheapest one you found. On top of that, you're also still trusting your partner to not have poked any holes in the condom.

Overall, It's still much better to be using the VPN than not, and if you trust your partner (i.e. the website or service you're going to), and you trust the VPN provider for whatever reason - perhaps a widely trusted company has given an independent audit of the VPN, or you or your workplace has set it up yourself - then for most situations you're pretty safe. Layering a VPN on top of the above tools is good, but layering VPNs on VPNs or on other networks is actually not dissimilar to layering condoms - it actually makes failure in very weird (and, lets face it, awkward) ways /more/ likely.

<h3>Safer Surfing</h3>
Still, though, wouldn't it be better if you could rely even less on trust, and have that trust backed up with evidence that you yourself can look at?

Using Tor is like using a condom which you not only know has gone through extensive testing, you can even visit the factory floor, look at the business' finances, and talk with the engineers and factory staff. It's /still/ not 100% safe, but it is a heck of a lot safer, and you can verify each and every claim made about what it does and does not do.

And to be clear here, if you're logging in to a website over Tor, that website now knows who you are (you're no longer anonymous to them, and possibly others watching you do this along the wire), and that website is storing your password and may fail to protect it at some point.  That website can still turn out to be malicious and attack you, and very powerful adversaries can even specifically try and intercept traffic coming from a website and going into the super-secret Tor network, change it, and include an attack they know works well against out of date versions of the browser you're using.  An out of date Tor browser is like an expired condom - it's best not to bet your life on it.

To really (over-)extend the analogy, the Tor-branded condom business happens to be heavily funded by a religious organization that is strongly against birth control (and indeed has an entire project that tries to undermine birth control methods, to the point of installing secret hole-punchers in condom factories).  This same organization (it's large!) does have a different and vocal component that strongly supports safer sex, and not only funds giving away condoms, but also the production of them.  It's not, seemingly, the most logical set up, but hey, we're talking religion, politics and sex - logic doesn't always come in to play here.

Like sex, there is no truly "safe" way to play on the Internet, and it's unrealistic to expect that abstinence from the Internet is realistic. So, be careful out there, adopt safer practices, and keep your wits about you.  Good luck!
