---
layout: page
title: Categories
---

The terms used on this site are defined on the pages linked below.

 <ul>
 {% assign sorted_posts = (site.categories.['aroha'] | sort: 'title') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

 <ul>
 {% assign sorted_posts = (site.categories.['terminology'] | sort: 'title') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
