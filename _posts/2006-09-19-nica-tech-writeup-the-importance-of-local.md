---
excerpt: "Sometimes, knowing the local context is not only important, but a stark
  requirement.  Scratch that - always.  In Managua, Nicaragua, this is point is driven
  home by the simple task of getting to where you're going.  A victim of earthquakes
  and politics, Managua is generally without reliable street signs, or addresses,
  but unlike, say, <a href=\"https://joncamfield.com/blog/2012.03/exploring_the_un_mappable\">Bangkok,
  where mapping is a futile attempt in capturing the ephemeral</a>, Managua simply
  doesn't have the structure to support creating a normal map.  \r\n\r\n<div style=\"float:right\"><img
  src=\"https://joncamfield.com/images/Mga-directions.png\"><br>Directions in Managua</div>\r\n\r\nSo
  the population has adapted.  Addresses in Managua are complex formulas of local
  history, community, and direction.  Cab drivers have a defined territory, and cross-town
  trips will result in your driver finding a \"local\" to help with the last few blocks.
  \ The cardinal directions are \"Al Lago\" - towards the lake, or North of the city
  - Up (East), Down (West) and to the mountains - Southish.  Then you specify the
  neighborhood, and then you go to landmarks.  Of course, back to the earthquake problem
  - those landmarks may not be there anymore.  \r\n\r\nThis particular recipe for
  an address is in the M. Lezcano neighborhood, and then from where the People's Bank
  used to be, 2 blocks towards the lake, and a 1/2 block east.  They get even crazier
  - <a href=\"https://www.npr.org/templates/story/story.php?storyId=4660766\">hairy
  handed women and broken down cars</a> are called out in this NPR interview.\r\n\r\nI
  digress, however.\r\n\r"
categories:
- ict4d


title: 'Nica Tech Writeup: The importance of local'
created: 1158709158
---
Sometimes, knowing the local context is not only important, but a stark requirement.  Scratch that - always.  In Managua, Nicaragua, this is point is driven home by the simple task of getting to where you're going.  A victim of earthquakes and politics, Managua is generally without reliable street signs, or addresses, but unlike, say, <a href="https://joncamfield.com/blog/2012.03/exploring_the_un_mappable">Bangkok, where mapping is a futile attempt in capturing the ephemeral</a>, Managua simply doesn't have the structure to support creating a normal map.  

<div style="float:right"><img src="https://joncamfield.com/images/Mga-directions.png"><br>Directions in Managua</div>

So the population has adapted.  Addresses in Managua are complex formulas of local history, community, and direction.  Cab drivers have a defined territory, and cross-town trips will result in your driver finding a "local" to help with the last few blocks.  The cardinal directions are "Al Lago" - towards the lake, or North of the city - Up (East), Down (West) and to the mountains - Southish.  Then you specify the neighborhood, and then you go to landmarks.  Of course, back to the earthquake problem - those landmarks may not be there anymore.  

This particular recipe for an address is in the M. Lezcano neighborhood, and then from where the People's Bank used to be, 2 blocks towards the lake, and a 1/2 block east.  They get even crazier - <a href="https://www.npr.org/templates/story/story.php?storyId=4660766">hairy handed women and broken down cars</a> are called out in this NPR interview.

I digress, however.

In August, I spent two weeks volunteering my IT services with <a href="https://www.esperanzaenaccion.org">Esperanza en Accion</a>, a non-profit in Managuat wor, Nicaragua that works on economically empowering Nicaraguan artisans, garment workers, and coffee farmers through fair trade practices.  They do incredibly good work, and it is mind-blowing to see the lifestyle changes in their artisans who have been able to pay for further education, afford needed medical bills for family members, and rebuild their board-and-cardboard houses with cinderblocks and other better materials in four short years, particularly in comparison to the many workers in Nicaragua's free trade export zone factories, who suffer from inhumane working conditions, union-busting businesses, and human rights violations. These things aside (!), they are not rebuilding their homes nor furthering their education, they are barely getting by.

<p>But I digress.  I feel that IT capacity building among these small non-profits is of huge value.  It's a bit removed from front-line development work, but in the two short weeks I was there I was able to greatly increase their workflow efficiency and capacity, which will enable them to do more with their current setup and to grow, hopefully, in the near term.</p>

<p>Some of this was just training in some relatively universal best practices; backing up, using some tools more efficiently, and so on - nothing particularly unique about it.  However, the most important parts are where traditional IT breaks down.  The electricity in Managua goes out, unpredictably, for 2-8 hours at a time, often in the middle of the afternoon.  Though they have a shared document folder, it is on the only "permanent" computer (i.e. non-personal laptop) in the office, which is a desktop plugged into an old UPS that doesn't last very long.  Ideally, some version control system on a remote Internet machine would be a great solution, but then the Internet can fail for up to months at a time, leading to huge problems with binary files (text files could just be merged, but .docs are binary and resist such useful things).  So we came up with a (human) process to save locally during power outages and replace on the server when the power returns. It's not perfect, <b>but it's locally relevant</b>.  This is, I feel, the real key to ICT development strategies - realizing when the "best practice" is contextually invalid for social or environmental externalities, whether they be hungry goats chewing on phone lines or cultural differences.</p>

<p>Free and open source tools also provided me with a great opportunity.  Not only are they reliably internationalized (all software has to be available in Spanish for obvious reasons), they are within the budget and customizable to local needs.  There's a lot more to say about OSS and ICT Dev, and I'll save that, and how I punched down ethernet jacks with my CVS keychain card, for another post.</p>
