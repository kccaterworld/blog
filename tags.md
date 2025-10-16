---
layout: default
title: Tags
permalink: /tags/
---

{% for tag in site.tags %}
  <h3 id="{{ tag[0] }}">Tag: {{ tag[0] }}</h3>
  <ul>
  {% for post in tag[1] %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
  </ul>
{% endfor %}