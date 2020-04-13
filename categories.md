---
layout: page
title: Categories
---

The content of this site is listed by category and linked below.

<h2>Aroha.dev</h2>

 <ul>
 {% assign sorted_posts = (site.categories.['aroha'] | sort: 'title') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

<h2>Art</h2>

 <ul>
 {% assign sorted_posts = (site.categories.['art'] | sort: 'title') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

<h2>Terminology</h2>

 <ul>
 {% assign sorted_posts = (site.categories.['terminology'] | sort: 'title') %}
{% for post in sorted_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
