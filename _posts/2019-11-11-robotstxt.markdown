---
layout: post
title:  "What is robots.txt and how have I configured it for my site?"
date:   2019-11-11 9:47:25 -0600
categories: jekyll update
author: Maryna
---

![robots-blog-image](/assets/pic/robots.png){:class="content-img"}

robots.txt is a TXT file put in the site root folder that contains instructions to be given to web robots that are trying to visit the site. 

When a robot tries to visit Web site URL it checks for robot.txt files in the site root folder and acts accordingly. 

<br>
While developing this website I also added robots.txt to the site root folder (/src), where I then specified the following instructions: 

<br>
User-agent: *

Disallow: /

<br>
The "User-agent: *" means this section applies to all robots. 

The "Disallow: /" means the robot can not visit any pages on this site.


