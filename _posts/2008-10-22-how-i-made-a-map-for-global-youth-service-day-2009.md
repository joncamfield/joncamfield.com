---
categories:
- ict4d
- web 2.0 and f/loss

title: How I made a map for Global Youth Service Day 2009
created: 1224700602
---
<p><strong>Series</strong>: <em><a href="">Overview</a> | <a href="http://www.joncamfield.com/blog/2008/10/drupal_and_maps_ii_modules_in_1.html">Modules</a> | <a href="http://www.joncamfield.com/blog/2008/11/drupal_and_maps_iii_getting_di.html">Structure and Taxonomies</a> | <a href="http://joncamfield.com/blog/2008/12/drupal_mapping_iii5_moving_up.html">On Drupal 6</a> | <a href="http://joncamfield.com/blog/2008/12/drupal_mapping_iv_filtering_an.html">Functionality</a></em></p>

<p>This is my "journal" of work in creating a user-modifiable map of the Global Youth Service Day events taking place around the world.  The goal was to create a map that staff non-techies could manage, non-techie youth and organizations from around the world could add to, and still (a) work and (b) be friendly to the techies managing it, allowing for mass import and so on.</p>

<div style="float: right; margin-left: 10px; margin-bottom: 10px;"><img alt="GYSD 2008 Event Map" src="/images/gysdmap.jpg" style="border: 2px solid black; width: 240px; height: 180px;"></a><br><span style="font-size: 0.9em; margin-top: 0px;">The GYSD Map in progress!</span></div>

<p>This is the first part of a series of entries (four or five probably).  This first one covers the overview and core software I'm using, and some discussion of why I've chosen what I have.  The next entry will cover modules and initial configuration work.</p>

<p>This guide is going to be a bit on the techie side, and I presume at least a bit of Drupal and webhosting experience when going through it, but nothing you can't google for help on from the community.  As a caveat, I'm also relatively new to drupal, this is only my third foray into the more complex worlds it offers.</p>

<p>I'm writing it down all in one place because almost every step I took fulfilled my 5 minute documentation rule (http://www.joncamfield.com/blog/2008/08/my_5_minute_rule_for_documenta.html), and because mapping is just darned useful as a visualization tool.  I don't think it's totally unreasonable for any nonprofit to reproduce my steps and get their own map, but having a techie on hand would certainly help.  <br />
</p>
                           </div>
                           <div id="more" class="entry-more">
                              <h3>The back-end</h3>

<p>I'm sure you can run this on just about anything.  I chose to use Drupal, and to put it on a basic LAMP system (LAMP means Linux/Apache/MySQL/PHP).  LAMP is a wonderful collection of open source technologies that interact beautifully.  As a non-profit, the free part is almost as important as the community and volunteer aspects of open source.  For a hosting provider, we went with DreamHost, which has a fantastic deal for 501(c)3 non-profits, and is generally a pleasure to work with as a web geek -- you can quickly and easily spin up new MySQL dbs, SSH logins, websites/subdomains/testing areas, and it has great automatic backups and integrated one-click Google Apps installation/support.</p>

<h3>Drupal and Friends</h3>
I chose Drupal 5, because at this time it seems to have the widest support in the module department.  Since beginning my project and now, Drupal 6 has really come into its own in terms of module support, and is a smoother and more powerful platform.  Regardless, look before you leap when deciding what version to go with (Drupal 7, with substantial improvements, is already available), because it's a lot easier to start out a site than to move it later.

<p>Drupal is one of the top two (ok, three) open source CMSes (Content Management Systems).  Joomla and Zope/Plone being the other two.  I feel Drupal is currently the leader in support and overall UX (User Experience), but your mileage might vary depending on your specific needs/goals.  Drupal is definitely more of a challenge to have work like a traditional website, but its internal structure is beautiful in its power and style, so I think it's worth the effort, and certainly will give you a new insight into your information architecture.</p>

<p>Also, if you forge ahead - let me let you in on a little secret of the Open Source tech world that's been of infinite use to me.  There's this old chat protocol called IRC - think of it as Instant Messenger chat rooms, but it predates IM by years, if not almost decades.  There's a IRC "server" which contains thousands of open source software specific chatrooms called Freenode.  You can find personal help on almost every topic imaginable here; with two caveats. First, do your homework before asking a question, as it's pretty rare for you to be the first person to have a problem with something, and it might already be solved.  Second, be patient and polite - these are often the lead developers, expert coders and the human life-force behind the software you're using -- and oftentimes they're doing it because they care about good software, not for a paycheck.  I'd give you step-by-step instructions to get in touch with these folk; but I think it's a good first step to google around to figure that out.</p>
