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
It really feels like an extension to the CSS language. It will let you use variables and other neat techniques to help
maintain the code easier and also prevent repeating the code. Having only to edit one variable to tweak a color that
you use more than once is really helpful. Especially if the website is really big. It also opens up the opportunity
to use functions. Now that is powerful.

Compared to regular CSS it feels less error prone, at least when using Jekyll and SASS. It keeps checking the code
and if you wrote an error in the CSS code it will stop the npm run watch and more or less yell at you. You can also
split the CSS code up to multiple files as much as you want because in the end you'll have one big CSS file for the
website.

When it comes to the techniques I used I would have to say I used variables a lot, I didn't have the time to use
functions yet but I will probably go back throughout the course and update the blog with the new things I learn.

Now for pros and cons I would have to say the pros are an easier way to maintain the code, the access to more powerful
techniques when writing the CSS code. Less error prone when writing the CSS code because the compiler will complain
about the code. Now for the cons. Longer compile time when more code is added, another entry point for bugs to be
introduced to the code.

####**What do you think of static site generators?**
Jekyll is so awesome and makes it so much easier to get a simple blog up and running. The fact that everything is
instantly updated when you save a document is helpful and the access to techniques like `% for post in site.posts limit:3  %`
is really helpful and opens up many opportunities.

The fact that it's so simple to get a blog up and running answers what type of websites site generators are suitable for.
Namely websites that don't use databases. Site generators are really only suitable for simple websites.

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
It's an initiative to help promote the people behind the website. Some owners don't want developers to add that
information directly to the website so having a .txt file that doesn't interfere with the code at all is an easy
and practical way to solve it.

I have configured the site with my name, my twitter, the site url, my location information.
I also wrote what components and software I've used in when developing the website and last some thanks to the
course teachers.

####**How did you implements comments to blog posts**
I choose to use Disqus which is a global comment system that lets you use other social media logins to comment on
the posts that you've choose to have it activated on. Why I choose it was because it's global, doesn't require
registration, and nowadays people have either a facebook or a twitter account, heck everyone has a google account
at least, so using Disqus was a really easy choice. It also wasn't that hard to install, set the page url and unique
identifier then embed the code to the post layout.

####**What is Open Graph and how do you make use of it?**
Open Graph lets you share you website on social medias more easily. It looks much better with image and the information
you want to share. It also allows the web page to have better functionality when shared on other sites, like facebook
for example. On facebook the web page will have the same functionality as any other object on facebook.

I have chosen to use the basic metadata with one optional metadata, description.
