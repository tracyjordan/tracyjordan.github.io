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


The blog posts of this site are listed below, with most recent first.

 <ul>
{% assign sorted_posts = (site.categories.['blog']  | sort: 'date') %}
{% for post in sorted_posts %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
