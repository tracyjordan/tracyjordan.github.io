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


Jez1
  
  
  3
  
   <ul>
 {% assign sorted_posts = (site.year.[2020] | sort: 'post_date') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
