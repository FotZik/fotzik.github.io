---
layout: page
title: Blog
permalink: /blog/
---

<h1 class="post-title">Blog posts</h1>

Here you'll be able to read all blog posts ever posted on the site.

<div class="home">
    
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
          <span class="post-meta">Posted: {{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
