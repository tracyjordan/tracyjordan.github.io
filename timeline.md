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
  
<h2>2020</h2>  
  
  {% assign sorted-posts = site.posts | where: "categories","2020" %}
{% for post in sorted-posts limit: 5 %}
  <li>{{post.title}}</li>
{% endfor %}

Jez1
