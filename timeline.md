---
layout: page
title: Timeline
---

The posts on this site are listed below in sequence from newer to older.

<ul>
{% assign sorted-posts = site.posts | sort: 'post_date' %}
  {% for post in sorted-posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title}}</a>
  </li>
  {% endfor %}
  </ul>
