---
excerpt: "<div style=\"float: right; margin-left: 10px; margin-bottom: 10px;\"><a
  \r\nhref=\"http://www.flickr.com/photos/dcmetroblogger/2026119441/in/set-72157594232448993/\"><img
  src=\"http://www.olpcnews.com/images/olpc-lcdc-mesh.jpg\" alt=\"olpc learning club\"
  style=\"border: 2px solid rgb(0, 0, 0); width: 200px; height: 197px;\"></a><br><span
  style=\"font-size: 0.9em; margin-top: 0px;\"><b>Time to mesh XOs</b></span></div>\r\n\r\n<p>Unless
  you're lucky enough to live within mesh range of many other XO users (or are part
  of an XO deployment or an <a href=\"http://roomtwelve.org\">innovative classroom
  project</a>, you probably have a pretty empty \"neighborhood,\" and look to Internet
  jabber servers to connect with other XOs. </p>\r\n\r\n<p>The state of the public
  jabber servers of recent has been in flux for a while, but seems to be settling
  down.</p>\r\n\r\n<p>XOChat.org seems to have disappeared from the Internet (any
  word on why?), and scouring the OLPC Wiki for <a \r\nhref=\"http://wiki.laptop.org/go/Community_Jabber_Servers\">community
  servers</a> has led to more dead ends than I care to relate. To be fair, I've mainly
  been using <a href=\"http://www.pidgin.im\">Pidgin.im</a> instead of my XO to test
  the networks out, and some servers, including <a \r\nhref=\"http://xoshare.org/mi/default.aspx\">XO1Share.org</a>,
  isn't playing nice  with my IM client - but does seem to have a decently vibrant
  community of XO users on it.  Jabber.laptop.org and jabber.sugarlabs.org are the
  other contenders currently (and jabber.laptop.org allows IM clients!, Sugarlabs
  throttles non-OLPC connections).</p>\r\n\r\n<p>There is also a scaling limitation
  in that any server can only take ~150 concurrent users.  </p>"
categories:
- olpc
- ict4d
tags:
- xo
- collaboration
- mesh
- jabber

title: Collaboration and the XO Mesh
created: 1247067999
---
<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a 
href="http://www.flickr.com/photos/dcmetroblogger/2026119441/in/set-72157594232448993/"><img src="http://www.olpcnews.com/images/olpc-lcdc-mesh.jpg" alt="olpc learning club" style="border: 2px solid rgb(0, 0, 0); width: 200px; height: 197px;"></a><br><span style="font-size: 0.9em; margin-top: 0px;"><b>Time to mesh XOs</b></span></div>

<p>Unless you're lucky enough to live within mesh range of many other XO users (or are part of an XO deployment or an <a href="http://roomtwelve.org">innovative classroom project</a>, you probably have a pretty empty "neighborhood," and look to Internet jabber servers to connect with other XOs. </p>

<p>The state of the public jabber servers of recent has been in flux for a while, but seems to be settling down.</p>

<p>XOChat.org seems to have disappeared from the Internet (any word on why?), and scouring the OLPC Wiki for <a 
href="http://wiki.laptop.org/go/Community_Jabber_Servers">community servers</a> has led to more dead ends than I care to relate. To be fair, I've mainly been using <a href="http://www.pidgin.im">Pidgin.im</a> instead of my XO to test the networks out, and some servers, including <a 
href="http://xoshare.org/mi/default.aspx">XO1Share.org</a>, isn't playing nice  with my IM client - but does seem to have a decently vibrant community of XO users on it.  Jabber.laptop.org and jabber.sugarlabs.org are the other contenders currently (and jabber.laptop.org allows IM clients!, Sugarlabs throttles non-OLPC connections).</p>

<p>There is also a scaling limitation in that any server can only take ~150 concurrent users.  </p>

<p>Regardless of what server you connect to (I'm usually on the XO1Share.org server when I'm on my OLPC),  I'd love to see more people hanging out and sharing applications and chat sessions.</p>

<h3>Connecting</h3>
<p>With the current build, it's easy (but requires a quick reboot) to change your jabber settings in <a href="http://wiki.laptop.org/go/Sugar_Control_Panel#Network">the 
control panel</a>. You can also change the jabber server from the command 
line:</p>
<ol>
  <li>type sugar-control-panel -g jabber<br />
    (this shows you the current setting)</li>
  <li>type sugar-control-panel -s jabber jabber.laptop.org<br />
    (this sets it to your new jabber server, replace jabber.laptop.org with whichever)</li>
  <li>Go back to the mesh view by pressing the ring button</li>
  <li>Other XO icons should pop up (sometimes slowly) if anyone's online! 
(Naturally, you also have to be connected to the Internet to mesh using Internet 
jabber servers)</li>
</ol>
<div style="float: right; margin-left: 10px; margin-bottom: 10px; width: 
180px;"><a href="http://www.flickr.com/photos/curiouslee/2976706457/"><img 
src="http://farm4.static.flickr.com/3203/2976706457_854aec1cfb_m.jpg" alt="Mike 
Lee shows off iPhone / XO chat" style="border: 2px solid rgb(0, 0, 0); width: 
180px; height: 240px;"></a><br><span style="font-size: 0.9em; margin-top: 
0px;"><b>Mike Lee shows off iPhone / XO chatting</b></span></div>
<p>You can also connect to most of the XO jabber servers using any IM client that supports the Jabber/XMPP 
protocol. I use  <a href="http://www.pidgin.im">Pidgin.im</a> (but have to re-create my account each time I connect). A downside here is that initially you sometimes get the XO user ID numbers, but right-clicking and selecting "Get Personal Info" retrieves the usernames.  IM clients don't automatically show up on the mesh view, but if that matters to you, there's a work-around for your OLPC to <a href="http://wiki.laptop.org/go/Jabber">better interact with IM clients</a>, and it's supposedly fixed in the 9.1 release (Sugar 0.84).</p>  

<p>Using your stogdgy old laptop or desktop to chat with XO users too boring?  Mike Lee discovered that you can <a href="http://www.olpcnews.com/forum/index.php?topic=3891.0">connect using  your iPhone</a> and posted a short <a href="http://www.flickr.com/photos/curiouslee/2976706457/">how-to on 
Flickr</a>:</p>
<blockquote>Anna has got Jabber running on an OLPC <a href="http://wiki.laptop.org/go/School_server" rel="nofollow">XS server</a> connecting to IM client software from the open Internet. Most any <a 
href="http://wiki.laptop.org/go/Jabber" rel="nofollow">Jabber</a> compatible client can now connect to a group of OLPC XO laptops using the same server. The Jabber client computers and XOs can be anywhere on the Internet. Here I'm using the <a href="http://www.palringo.com/" rel="nofollow">Palringo</a> chat client on my iPhone to connect to the <a href="http://wiki.laptop.org/go/Chat" rel="nofollow">Chat Activity</a> on the XO laptop next to it here in Wheaton, MD, but using wifi and by way of Birmingham, Alabama.</blockquote>

<br clear="right" />
<h3>Where next?</h3>
<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a 
href="http://flickr.com/photos/dcmetroblogger/2288483805/"><img 
src="http://farm4.static.flickr.com/3098/2288483805_45c0bce779_m.jpg" alt="Join OLPC mesh activities" style="border: 2px solid rgb(0, 0, 0); width: 240px; "></a><br><span style="font-size: 0.9em; margin-top: 0px;"><b>Join local activities!</b></span></div>

<p>There's some great ideas on XO chatting going on in the OLPC Forums, like <a href="http://olpcnews.com/forum/index.php?topic=2817.0" target="_blank">recurring, scheduled chats</a> and a <a href="http://olpcnews.com/forum/index.php?topic=2434.15" target="_blank">Who's who list</a> to link XO handles to people.  Some interesting ideas for using the mesh that I saw on xochat.org server while it was up ranged from basic group chats to a public quote-file maintained by a shared Write activity.  XO1share currently is maintaining a share document with the locations (city/state/country) of who's connecting regularly. Arbor Heights Elementary School has a <a href="http://www.roomtwelve.org">third grade class</a> posting and chatting using XOs (more info at <a href="http://xoclassroom.wikispaces.com">XOClassroom.com</a>) and of course Anna's <a href="http://alabamaxo.org">AlabamaXO School Server</a> showcasing some educational models for XO usage in the U.S.A.</p>

<p>What's your innovative idea for using the XO jabber/mesh system? What server do you use most often?</p>
