---
excerpt: "I missed the recent <a href=\"https://technologysalon.org/2009/05/m-development-challenge.html\">Technology
  Salon on Mobiles for Development</a> (I was kind of busy with <a href=\"https://GYSD.org\">Global
  Youth Service Day</a>), and was already scheduled to make it to the <a href=\"https://mobileactive.org/\">Mobile
  Active m4Change</a> unconference the next week.\r\n\r\nA prime outcome of the Tech
  Salon was a challenge from Vodafone's <a href=\"https://www.vodafone.com/start/about_vodafone/corporate_governance/executive_committee/terry_kramer.html\">Terry
  Kramer</a>: \r\n\r\n<blockquote>Mobile network operators (MNO) want increase revenues
  and market share by expanding into rural areas, and see partnerships with the development
  community as a key market entry strategy. Specifically, Vodafone is looking to the
  development community for key applications that solve a common need for many and
  can be scaled into commercial activities.</blockquote>\r\n\r\nHere's my response,
  an idea that's been rattling around in my head for quite some time.\r\n\r\n<div
  style=\"float: right; margin-left: 10px; margin-bottom: 10px;\"><a href=\"https://www.flickr.com/photos/phauly/399692232/\"><img
  src=\"https://farm1.static.flickr.com/168/399692232_fedd542c2c_m_d.jpg\" alt=\"An
  openMoko Linux Phone\" style=\"border: 2px solid rgb(0, 0, 0);\" width=\"240\" height=\"180\"><br><span
  style=\"font-size: 0.9em; margin-top: 0px;\">This would be easier on open platforms...</div>A
  common \"form\" application to send out encoded questions and receive back answers
  via SMS.\r\n\r\nThe core would be an agreed-upon encoding/compression format for
  sending form questions and receiving the answers via SMS.\r\n\r\nThis standard could
  be coded to using existing outreach tools like EpiSurveyor, FrontlineSMS, RapidSMS,
  and the like.  It would have a \"server-side\" component where you could set up
  a form, specify the answer types (y/n (or t/f), multiple choice, very-short-answer?)
  and compose the SMS messages to send.\r\n\r\nThe key (and the hard part) is having
  this app as common as a calculator tool on deployed phones.  The app would capture
  the coded SMS form, present it as a user-friendly form, and take the answers and
  reply (again via SMS) using as few outbound messages as possible.\r\n\r\nAnyone
  with an SMS-sending tool could code questions and use their tool to distribute them;
  and any phone with this (pre-installed) app could \"decrypt\" the compacted form
  and present it to the user.\r\n\r\nThis would make data collection much smoother,
  eliminate distribution of questionnaires and codesheets prior to each new questionnaire,
  and improve data quality.  \r\n\r\nI see immediate applications in election obersvation,
  human rights monitoring, and health field-worker reporting, not to mention census,
  and even for-profit ventures for immediate customer satisfaction surveys, more complex
  SMS-voting (imagine what BravoTV would do with this were it widely deployed!)\r\n"
categories:
- mobile4dev
tags:
- sms
- mobile
- health
- m4d
- m4change
- election observation

title: 'Blue-skying Mobile Apps: Common Forms'
created: 1241539525
---
I missed the recent <a href="https://technologysalon.org/2009/05/m-development-challenge.html">Technology Salon on Mobiles for Development</a> (I was kind of busy with <a href="https://GYSD.org">Global Youth Service Day</a>), and was already scheduled to make it to the <a href="https://mobileactive.org/">Mobile Active m4Change</a> unconference the next week.

A prime outcome of the Tech Salon was a challenge from Vodafone's <a href="https://www.vodafone.com/start/about_vodafone/corporate_governance/executive_committee/terry_kramer.html">Terry Kramer</a>: 

<blockquote>Mobile network operators (MNO) want increase revenues and market share by expanding into rural areas, and see partnerships with the development community as a key market entry strategy. Specifically, Vodafone is looking to the development community for key applications that solve a common need for many and can be scaled into commercial activities.</blockquote>

Here's my response, an idea that's been rattling around in my head for quite some time.

<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><a href="https://www.flickr.com/photos/phauly/399692232/"><img src="https://farm1.static.flickr.com/168/399692232_fedd542c2c_m_d.jpg" alt="An openMoko Linux Phone" style="border: 2px solid rgb(0, 0, 0);" width="240" height="180"><br><span style="font-size: 0.9em; margin-top: 0px;">This would be easier on open platforms...</div>A common "form" application to send out encoded questions and receive back answers via SMS.

The core would be an agreed-upon encoding/compression format for sending form questions and receiving the answers via SMS.

This standard could be coded to using existing outreach tools like EpiSurveyor, FrontlineSMS, RapidSMS, and the like.  It would have a "server-side" component where you could set up a form, specify the answer types (y/n (or t/f), multiple choice, very-short-answer?) and compose the SMS messages to send.

The key (and the hard part) is having this app as common as a calculator tool on deployed phones.  The app would capture the coded SMS form, present it as a user-friendly form, and take the answers and reply (again via SMS) using as few outbound messages as possible.

Anyone with an SMS-sending tool could code questions and use their tool to distribute them; and any phone with this (pre-installed) app could "decrypt" the compacted form and present it to the user.

This would make data collection much smoother, eliminate distribution of questionnaires and codesheets prior to each new questionnaire, and improve data quality.  

I see immediate applications in election obersvation, human rights monitoring, and health field-worker reporting, not to mention census, and even for-profit ventures for immediate customer satisfaction surveys, more complex SMS-voting (imagine what BravoTV would do with this were it widely deployed!)
<!--break-->
