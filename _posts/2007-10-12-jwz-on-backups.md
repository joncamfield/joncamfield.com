---
excerpt: |-
  <p>JWZ as usual offers good, if acerbic, advice; today on <a href="https://jwz.livejournal.com/801607.html">backups</a>:</p>


   I am here to tell you about backups. It's very simple.

  <p>Option 1: Learn not to care about your data. Don't save any old email, use a film camera, and only listen to physical CDs and not MP3s. If you have no posessions, you have nothing to lose. <br />
  [...]</p>

  <p>Put one of these drives in its enclosure on your desk. Name it something clever like "Backup". If you are using a Mac, the command you use to back up is this:</p>
categories:
- ict4d
- ict policy

title: JWZ on backups
created: 1192217074
---
<p>JWZ as usual offers good, if acerbic, advice; today on <a href="https://jwz.livejournal.com/801607.html">backups</a>:</p>


 I am here to tell you about backups. It's very simple.

<p>Option 1: Learn not to care about your data. Don't save any old email, use a film camera, and only listen to physical CDs and not MP3s. If you have no posessions, you have nothing to lose. <br />
[...]</p>

<p>Put one of these drives in its enclosure on your desk. Name it something clever like "Backup". If you are using a Mac, the command you use to back up is this:</p>

<p>sudo rsync -vaxE --delete --ignore-errors / /Volumes/Backup/</p>

<p>If you're using Linux, it's something a lot like that. If you're using Windows, go fuck yourself. </p>

<p>NB: There are ways to do this in Windows, too.  Not as simply, mind you, but it can work.</p>
