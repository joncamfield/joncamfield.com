---
excerpt: "(Or, how to remind anyone snooping your email of your fourth amendment rights)"
categories:
- hactivismo
- human rights
tags:
- nsa
- echelon

header:
  overlay_image: /assets/images/exchelontext.png
  teaser: /assets/images/exchelontext.png
  caption: "Stylized Jam ECHELON keywords"


title: Jam Echelon Day, Redux
created: 1381528367
---
(Or, how to remind anyone snooping your email of your fourth amendment rights)

So clearly we have a situation here where we failed to learn from the past.  <a href="http://www.wired.com/politics/law/news/1999/10/32039">Fourteen years ago</a> (Exactly in a few days - Oct 21!), we were protesting ECHELON, which was (is) a "worldwide computer spy network [that] reportedly scans all email, packet traffic, telephone conversations, and more in an effort to ferret out potential terrorist or enemy communications. Once a communication is plucked from the electronic cloud, certain keywords allegedly trigger a recording of the conversation or email in question."

In response (along with a short burst in activity around people trying to figure out how to use <a href="http://www.gnupg.org/">PGP</a>), hackers added amusing bonus keywords in the parts of emails that humans rarely see (where junk like the path the email took, listserv details, and so on goes) - many, including myself, added the 4th Amendment to the US Constitution, as well as participating in "Jam Echelon day," when everyone added what we presumed at the time were these mythical "trigger words:"

<blockquote>ATF DOD WACO RUBY RIDGE OKC OKLAHOMA CITY MILITIA GUN HANDGUN MILGOV ASSAULT RIFLE TERRORISM BOMB DRUG KORESH PROMIS MOSSAD NASA MI5 ONI CID AK47 M16 C4 MALCOLM X REVOLUTION CHEROKEE HILLARY BILL CLINTON GORE GEORGE BUSH WACKENHUT TERRORIST.</blockquote>

As an aside: maannnnnn, do you remember the 90s? Was that an unpleasant walk down memory lane or what?

Anyhow, this amusing idea that this would work for more than a few minutes just doesn't seem to die, and someone's trying it with a new "security" tool called <a href="http://rt.com/usa/scaremail-nsa-tool-nonsense-957/">ScareMail</a> that "takes keywords from an extensive US Department of Homeland Security list used to troll social media websites and utilizes them “to disrupt the NSA’s surveillance efforts by making NSA search results useless.” "

While that's ... well, whatever.  It's a nice thought, right?  Probably not very useful overall.  Anyhow, it gives me a small boost of civic pride to tweak my email settings and put the fourth amendment text back in to almost every email I send out.  This requires an actual email client (Thunderbird works nicely), and some configuration hacking:

<ul>
<li>Go to  Edit → Preferences → Advanced → General → Config editor</li>
<li>Right click, new, "string"</li>
<li>For 'Enter the preference name' use "mail.identity.id1.header.header1"</li>
<li>For the string, add "X-Fourth-Amendment: The right of the people to be secure in their persons, houses, papers, and effects, against unreasonable searches and seizures, shall not be violated, and no Warrants shall issue, but upon probable cause, supported by Oath or affirmation, and particularly describing the place to be searched, and the persons or things to be seized."</li>
<li>If you have multiple mail accounts, you'll have to do this for each one, using id2, id3, etc. and header2, header3, etc.  </li>
<li>Restart thunderbird, make sure you didn't break anything.  For more details, peek at http://kb.mozillazine.org/Custom_headers</li>
</ul>
<!--break-->
