---
layout: default
title: All Posts
permalink: /posts/
---

# All Posts

<ul>
{% for post in site.posts %}
  <li>
    <span>{{ post.date | date: "%B %d, %Y" }}</span> - 
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>