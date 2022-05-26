---
excerpt: "<strong>Update: </strong> Hello readers from Alanna's post on the OLPC at
  <a href=\"https://undispatch.com/node/8859\">UNDispatch</a> - You should check my
  original article on the OLPC TCO - written back in 2006 - over at <a href=\"https://www.olpcnews.com/sales_talk/price/the_real_cost_of_the.html\">OLPCNews.com</a>.\r\n\r\nIf
  you poke around enough on the Laptop.org wiki, you find a few interesting corners.
  \ Linked from their work in creating a training and reference document for OLPCCorps,
  a link to <a href=\"https://wiki.laptop.org/go/Deployment_Guide/Workbook\">an Excel
  spreadsheet to calculate OLPC-specific costs for a deployment</a>, which has been
  created and maintained by OLPC's John Watlington\r\n"
categories:
- olpc
tags:
- tco
- laptop
- "$972"

title: It's Raining OLPC TCOs (1 of 4)
created: 1249394317
---
<strong>Update: </strong> Hello readers from Alanna's post on the OLPC at <a href="https://undispatch.com/node/8859">UNDispatch</a> - You should check my original article on the OLPC TCO - written back in 2006 - over at <a href="https://www.olpcnews.com/sales_talk/price/the_real_cost_of_the.html">OLPCNews.com</a>.

If you poke around enough on the Laptop.org wiki, you find a few interesting corners.  Linked from their work in creating a training and reference document for OLPCCorps, a link to <a href="https://wiki.laptop.org/go/Deployment_Guide/Workbook">an Excel spreadsheet to calculate OLPC-specific costs for a deployment</a>, which has been created and maintained by OLPC's John Watlington
<!--break-->
<h2>Better late than never?</h2>

I've been beating the drum since <a href="https://www.olpcnews.com/sales_talk/price/the_real_cost_of_the.html">November 2006</a> on the importance of including the costs for the full environment that the XO laptop needs to thrive.  Implementation planning has to move beyond the per-unit cost, it must include the solution for charging the laptops, host the more power-hungry XS server, extend the mesh network to the community, and connect to the Internet at least occasionally.  And that doesn't even touch the costs of curricula development, teacher training, and institutional changes for distribution, maintenance, even testing.

<h3>My 2006 TCO</h3>

I got into a good amount of hot water by proposing that the cost of OLPC projects went beyond (number of students)×($100).  The magic number was <a href="https://www.olpcnews.com/sales_talk/price/the_real_cost_of_the.html">$972/laptop for a 5-year project</a>.  Widely decried, a few much more in-depth explorations revealed that my back-of-the-envelope TCO calculation was actually <a href="https://www.olpcnews.com/implementation/plan/cost_of_olpc_in_haiti.html">pretty close</a>.

<h3>GeSCI 1:1 TCO</h3>

Roxana Bassi and I worked on a tool which any implementing group could plug in local numbers while being led through increasingly complex worksheets which provided calculations for every level of the school system, whether you were concerned about per-school costs or system-wide expenses.  

https://www.gesci.org/ict-infrastructure-connectivity-and-accessibility.html (<a href="https://www.gesci.org/old/files/docman/TCO-oneone-manual.pdf">Guide</a> and <a href="https://www.gesci.org/old/files/docman/TCO-oneone.xls">Worksheet</a>)

<h3>Consultant TCOs</h3>

At the same time, <a href="https://www.vitalwaveconsulting.com/insights/articles-presentations.htm">VitalWave also came out with a TCO calculation</a> comparing different approaches (1:1 computing, computer labs, etc.) with special attention to the OLPC in the 1:1 model. The VitalWave paper was covered in a <a href="https://www.olpcnews.com/implementation/plan/total_cost_of_ownership_seminar.html">World Bank e-Development webinar</a> last November.  NComputing also has a <a href="https://www.ncomputing.com/Portals/0/Calculator/NComputing%20Purchase-TCO-Green%20Calculator%206-12-08%20rev%202.2.xls">TCO calculcator</a> that brings in environmental concerns to showcase the value of their low-power terminal systems.

<h2>And now ... the OLPC TCO?</h2>

The Laptop.org tool at https://wiki.laptop.org/go/Deployment_Guide/Workbook seems to be a relative of the GeSCI tool in its approach, but cuts out some  1:1 computing calculations which are irrelevant to the XO laptop, and adds in other calculations specific to the XO to help plan for the maximum power draw while charging.

This is a great tool, and it's unfortunate that it wasn't part of the
OLPC discussion from the beginning; joining the open source ideals of their
design process with the rather closed business process.

It also reveals some of the presumptions being made in the design and implementation processes - the list of Internet connectivity options range from DSL and VSAT to "none", and call out specific cellular connectivity options, but don't even mention plain dial-up (there is an "other" category).

The following blog entries will present these various calculations head-to-head, first outlining what we will compare (and why) and then running the numbers to see both what the current cost of OLPC deployments are, and to reveal differences between the various tools.
