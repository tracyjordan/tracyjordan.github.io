---
layout: page
title: Timeline
---

The posts on this site are listed below in sequence from newer to older.

<ul>
{% assign sorted-posts = site.posts | sort: 'date' %}
  {% for post in sorted-posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title}}</a>
  </li>
  {% endfor %}
  </ul>


{% assign sorted-posts = site.posts | sort: 'post_date' | reverse %}
{% assign featured-posts = sorted-posts | where_exp:"post","post.featured" %}
{% for post in featured-posts limit:3 %}
  <h2><a href="{{ post.url }}">{{ post.title | truncate: 58 }}</a></h2>
{% endfor %}
