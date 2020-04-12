---
layout: page
title: Timeline
---

The posts on this site are listed below in sequence from newer to older.

{% assign sorted-posts = site.posts | sort: 'date' %}
  {% for post in sorted-posts %}
  <ul><li>
    <a href="{{ post.url }}">{{ post.title}}</a>
  </li></ul>
  {% endfor %}
