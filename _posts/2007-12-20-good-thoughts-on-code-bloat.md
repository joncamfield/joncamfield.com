---
excerpt: |-
  <p><a href="https://steve-yegge.blogspot.com/2007/12/codes-worst-enemy.html">Steve Yegge writes on code bloat</a>:</p>

  I recently had the opportunity to watch a self-professed Java programmer give a presentation in which one slide listed Problems (with his current Java system) and the next slide listed Requirements (for the wonderful new vaporware system). The #1 problem he listed was code size: his system has millions of lines of code. [...]

  <p>So I was really glad to see that this guy had listed code size as his #1 problem.</p>
categories:
- ict4d
- tinkering


title: Good thoughts on code bloat
created: 1198165646
---
<p><a href="https://steve-yegge.blogspot.com/2007/12/codes-worst-enemy.html">Steve Yegge writes on code bloat</a>:</p>

I recently had the opportunity to watch a self-professed Java programmer give a presentation in which one slide listed Problems (with his current Java system) and the next slide listed Requirements (for the wonderful new vaporware system). The #1 problem he listed was code size: his system has millions of lines of code. [...]

<p>So I was really glad to see that this guy had listed code size as his #1 problem.</p>

<p>Then I got my surprise. He went on to his Requirements slide, on which he listed "must scale to millions of lines of code" as a requirement. Everyone in the room except me just nodded and accepted this requirement. I was floored.</p>

<p>Why on earth would you list your #1 problem as a requirement for the new system? I mean, when you're spelling out requirements, generally you try to solve problems rather than assume they're going to be created again. So I stopped the speaker and asked him what the heck he was thinking.</p>

<p>His answer was: well, his system has lots of features, and more features means more code, so millions of lines are Simply Inevitable. "It's not that Java is verbose!" he added â€“ which is pretty funny, all things considered, since I hadn't said anything about Java or verbosity in my question.</p>

<p>The thing is, if you're just staring in shock at this story and thinking "how could that Java guy be so blind", you are officially a minority in the programming world. An unwelcome one, at that.</p>
