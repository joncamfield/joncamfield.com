---
excerpt: |-
  <p>So, this weekend I thought it'd be a great time to upgrade to the latest joyride builds, which are rumored to have solved the earlier record problems, and hopefully the SD card corruption issues as well.    This is supposed to be an only-mildly-painful experience, with a few command line tricks, a few boot tricks, and so on.  Nothing serious.<br />
  <a href="http://xkcd.com/349/h" target="_blank"></a><br clear="all" /><b>XKCD on upgrading difficulties (and sharks)</b>
categories:
- ict4d
- olpc


title: OLPC joyride no so joyful (or, what Jon did all day Sunday)
created: 1216053644
---
<p>So, this weekend I thought it'd be a great time to upgrade to the latest joyride builds, which are rumored to have solved the earlier record problems, and hopefully the SD card corruption issues as well.    This is supposed to be an only-mildly-painful experience, with a few command line tricks, a few boot tricks, and so on.  Nothing serious.<br />
<a href="http://xkcd.com/349/h" target="_blank"></a><br clear="all" /><b>XKCD on upgrading difficulties (and sharks)</b><br />
And, in fact, it updated just fine.  I wasn't too impressed at the increased speed that's been promised, but the UI had a few enhancements, and I was looking forward to improved power management.</p>

<p>Now, I use my OLPC for about 4 main tasks - taking notes, checking email/Internet, playing Implode, and watching movies on planes (and TED talks on the Metro!).  All tasks I find the XO to excel at, frankly - it's light yet rugged enough to always carry, and with the great wifi reception and sun-readable screen, it's rare that I can't make full use of the XO; whether I'm at the park, home, or near anyone with an open wifi connection.</p>

<p>Booting into the new joyride build I find many improvements to the UI and network views, some that were interesting but neither exciting nor bad, and that mplayer doesn't work for me.  In fact, it causes a hard crash.  Same with Record, Measure, TamTam.... basically anything fancy.  The activity loads, but whenever it tries to actually play the video or activate the camera or mic, it freezes.  The wifi lights continue to flicker, and the battery light will change state, but no keyboard or mouse response.</p>

<p>I thought this was an unfortunate joyride issue, and restored back to 703 using olpc-update; same problem.  I then did a secure reflash from USB (twice!) and tried an olpc-update from there to restore functionality, but no luck.  Booting into open firmware and running test /camera provided a moving camera image, so it's not (thankfully!) a hardware problem; and I don't think it's the activities themselves (I downloaded a Record from the Activities page to test).  If I had to guess, I'd think it was a driver/module problem or at the X level, but I'm not familiar enough with Linux or Sugar to really diagnose or fix that.</p>

<p>I continued to muck around in discussion with some folks on the irc.freenode.net #OLPC-help channel, and sent an email into the support gang at laptop.org.  cjb suggested I try yet another reflash, starting from a completely blank slate - reformatted USB stick, dowloading a new image, everything.  The second time I tried <b>that</b>, it magically took and started working.  Continued discussion with the support gang indicated that sometimes the reflashing doesn't fully take, especially when going backwards in builds.</p>

<p>Needless to say, I might wait a while before going on another joyride. <br />
</p>
