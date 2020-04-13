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

 <ul>
 {% assign sorted_posts = (site.categories.['2020'] | sort: 'date') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>



Jez1
