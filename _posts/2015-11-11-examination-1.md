---
layout: post
title:  "Reflection on the first examination"
date:   2015-11-11
comments:   true
disqus_identifier: 201511112250
categories: examination
---
In examination 1 we were required to answer 6 questions regarding the process of setting up the examination, and what
we thought about it. Some of the questions also target information brought up during the first lecture.

####**The 6 questions are:**
1. What do you think of pre-compiling your CSS?
 * Compare to regular CSS
 * Which techniques did you use?
 * Pros and cons?
2. What do you think of static site generators?
 * What type of projects are they suitable for?
3. What is robots.txt and how have you configured it for your site?
4. What is humans.txt and how have you configured it for your site?
5. How did you implements comments to blog posts?
6. What is Open Graph and how do you make use of it?

So here are my answers to the questions above.

####**What do you think of pre-compiling your CSS?**
Pre-compiling your CSS lets you use variables in CSS code. Meaning you can do less DRY and makes it easier to maintain
the CSS code.

####**What do you think of static site generators?**


####**What is robots.txt and how have you configured it for your site?**
robots.txt is a way to control what search robots can and cannot index. You can disallow certain folders and files
from being indexed. You can also exclude a single robot if wanted.

{% highlight html %}
User-agent: *
Disallow: /
{% endhighlight %}
This will make all robots `User-agent: *` not be able to index any files in `/` which is the root, so that would mean
all files with the above code.

To exclude a single robot swap out * for the robot that you want to exclude. Example `User-agent: Google` will
exclude Google.

To exclude a file swap out / for the file structure. Example `/junk.html` will exclude the junk.html file.

For this site I decided not to allow any robots to index anything. The reason for this is because I want the blog
to be private and only open to myself, my fellow students and the teachers.

####**What is humans.txt and how have you configured it for your site?**


####**How did you implements comments to blog posts**


####**What is Open Graph and how do you make use of it?**

