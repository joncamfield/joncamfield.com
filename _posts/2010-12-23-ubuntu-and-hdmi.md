---
excerpt: '<div class=''posterous_autopost''><p>Lazywebs, here is an answer. &nbsp;Having
  problems with a black/blank/undetected screen on your HDMI out in Ubuntu? &nbsp;Using
  x86_64 and Nvidia? &nbsp;Here''s two tricks I discovered. &nbsp;I''m failing at
  being a good netizen and digging up the tens of various threads on similar problems,
  creating/remembering/resetting my accounts and posting my solution there, but hopefully
  the magic of google will lead fellow lost souls here. &nbsp;</p>  <p>If none of
  this makes any sense, get back to your eggnog.</p>  <p>In a (successful!) attempt
  to hook my Lenovo y550 laptop running Ubuntu 10/Maverick Meercat to my parents 720p
  HD TV via the HDMI port, I encountered an unusual (this used to work fine!) number
  of errors, and a lot of dead ends. &nbsp;The first being finding an HDMI cable out
  here. After a grueling run through the various big-box stores, selling the damned
  thing for $40 and waay up (they cost <a href="https://www.amazon.com/gp/product/B0002L5R78?ie=UTF8&amp;tag=joncamfield-20&amp;linkCode=as2&amp;camp=1789&amp;creative=390957&amp;creativeASIN=B0002L5R78">under
  $6 on Amazon.com</a>), I peeked into the <a href="https://www.sanangeloav.com/">neighborhood
  A/V shop</a> near my cousins'' (two cousins, one shop) western-ware store. &nbsp;He
  gave me a fair price for an unbagged, ~1m cable: free. &nbsp;I love small town economies
  where customer referral and satisfaction are more important that 10 cents of profit.</p>  <p>&nbsp;</p>'
categories: 
- tinkering


title: Ubuntu and HDMI
created: 1293145628
---
<div class='posterous_autopost'><p>Lazywebs, here is an answer. &nbsp;Having problems with a black/blank/undetected screen on your HDMI out in Ubuntu? &nbsp;Using x86_64 and Nvidia? &nbsp;Here's two tricks I discovered. &nbsp;I'm failing at being a good netizen and digging up the tens of various threads on similar problems, creating/remembering/resetting my accounts and posting my solution there, but hopefully the magic of google will lead fellow lost souls here. &nbsp;</p>  <p>If none of this makes any sense, get back to your eggnog.</p>  <p>In a (successful!) attempt to hook my Lenovo y550 laptop running Ubuntu 10/Maverick Meercat to my parents 720p HD TV via the HDMI port, I encountered an unusual (this used to work fine!) number of errors, and a lot of dead ends. &nbsp;The first being finding an HDMI cable out here. After a grueling run through the various big-box stores, selling the damned thing for $40 and waay up (they cost <a href="https://www.amazon.com/gp/product/B0002L5R78?ie=UTF8&amp;tag=joncamfield-20&amp;linkCode=as2&amp;camp=1789&amp;creative=390957&amp;creativeASIN=B0002L5R78">under $6 on Amazon.com</a>), I peeked into the <a href="https://www.sanangeloav.com/">neighborhood A/V shop</a> near my cousins' (two cousins, one shop) western-ware store. &nbsp;He gave me a fair price for an unbagged, ~1m cable: free. &nbsp;I love small town economies where customer referral and satisfaction are more important that 10 cents of profit.</p>  <p>&nbsp;</p>  <p>OK, back to the geekiness. I had to grab the <a href="https://www.nvidia.com/object/unix.html">latest drivers from nvidia</a>&nbsp;(260.19.29), drop out of X and stop gdm, install those drivers, and reboot. &nbsp;This got me to detecting the TV, but no matter what configuration I tried, I just couldn't activate it. &nbsp;In desperation, I moved on to using the nvidia-settings tool to start mucking with my xorg.conf file, and it threw a permissions error. &nbsp;I backed down but realized that this might be the core problem. &nbsp;Up comes a terminal to sudo nvidia-settings to run it with root permissions, and magically the screen started working when I re-applied the TwinView settings. &nbsp;&nbsp;</p>  <p>That's all. &nbsp;From there on out, it was smooth sailing.</p></div>
