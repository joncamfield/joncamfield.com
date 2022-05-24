---
excerpt: "<p>So, Amazon now forces you to use their download tool.  Which seems silly.
  \ But they offer a Linux version, which is nice.  But it only is built for 32 bit
  architectures.  Which is unfortunate.  There's a way around that, however!  Thanks
  to the efforts of <a href=\"http://www.ensode.net/roller/dheffelfinger/entry/installing_amazon_mp3_downloader_under\">these</a>
  <a href=\"http://threebrothers.org/brendan/blog/amazon-mp3-downloader-on-64-bit-ubuntu-lucid-lynx/\">two</a>,
  the handy getlibs tool, and the fact you can turn back time and get previous copies
  of libraries, it takes only a few minutes to get downloading.  I've put their tools
  together into this script, after the jump:</p>\r\n"
categories:
- tinkering
tags:
- ubuntu
- amd64

title: "#Ubuntu Tips: Amazon MP3 Downloads"
created: 1296922686
---
<p>So, Amazon now forces you to use their download tool.  Which seems silly.  But they offer a Linux version, which is nice.  But it only is built for 32 bit architectures.  Which is unfortunate.  There's a way around that, however!  Thanks to the efforts of <a href="http://www.ensode.net/roller/dheffelfinger/entry/installing_amazon_mp3_downloader_under">these</a> <a href="http://threebrothers.org/brendan/blog/amazon-mp3-downloader-on-64-bit-ubuntu-lucid-lynx/">two</a>, the handy getlibs tool, and the fact you can turn back time and get previous copies of libraries, it takes only a few minutes to get downloading.  I've put their tools together into this script, after the jump:</p>
<!--break-->
<blockquote><code><textarea cols="80" rows="25">
# First, let's get getlibs
sudo apt-get install getlibs

# Download  Amazon's deb
wget http://amazonm-002.vo.llnwd.net/u/d1/clients/en_US/1.0.9/amazonmp3_1.0.9~ibex_i386.deb?httpHeader%5FContent-Disposition=attachment%3B%20filename%3Damazonmp3.deb&amp;marketplace=1

# Forcefully install it
sudo dpkg -i --force-all amazonmp3.deb

# Run Getlibs for the available packages
sudo getlibs /usr/bin/amazonmp3

# Get the libboost ones
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/b/boost/libboost-filesystem1.34.1_1.34.1-11ubuntu1_i386.deb
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/b/boost/libboost-regex1.34.1_1.34.1-11ubuntu1_i386.deb
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/b/boost/libboost-date-time1.34.1_1.34.1-11ubuntu1_i386.deb
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/b/boost/libboost-signals1.34.1_1.34.1-11ubuntu1_i386.deb
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/b/boost/libboost-iostreams1.34.1_1.34.1-11ubuntu1_i386.deb
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/b/boost/libboost-thread1.34.1_1.34.1-11ubuntu1_i386.deb
sudo getlibs -w http://old-releases.ubuntu.com/ubuntu/pool/main/i/icu/libicu38_3.8.1-2ubuntu0.2_i386.deb

# Let's do a final check
sudo getlibs /usr/bin/amazonmp3

#run amazonmp3 to connect it to your default browser!
</textarea></code></blockquote>
