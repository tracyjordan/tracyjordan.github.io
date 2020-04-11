---
layout: page
title: Timeline
---

The posts on this site are listed below in sequence from newer to older.


  {% for post in site.posts %}
  <ul><li>
    <a href="{{ post.url }}">{{ post.title }}</a> {{ post.date | date_to_rfc822 }} (NZ)
  </li></ul>
  {% endfor %}
