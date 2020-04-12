---
layout: page
title: Timeline
---

The posts on this site are listed below in sequence from newer to older.

  {% for post in site.posts | sort: 'date' %}
  <ul><li>
    <a href="{{ post.url }}">{{ post.title}}</a>
  </li></ul>
  {% endfor %}


{% assign sorted-posts = site.posts | sort: 'date' %}
  {% for post in sorted-posts %}
  <ul><li>
    <a href="{{ post.url }}">{{ post.title}}</a>
  </li></ul>
  {% endfor %}
  
  Jez3
