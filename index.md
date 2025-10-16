---
title: Welcome to my blog
---

# I have a blog now!

I've had this idea for a while, and I finally got it to work. This is my blog, where I'll be posting about various topics that interest me. Feel free to request stuff.

I'll do my best to update somewhat regularly, but who knows if I'll actually do that.

## Navigation

[View all tags](/tags/)

[View all posts](/posts/)

## All Blog Posts

<ul>
{% for post in site.posts %}
  <li>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <span>{{ post.date | date: "%B %d, %Y" }}</span>
    <p>{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>