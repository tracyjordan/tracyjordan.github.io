---
layout: page
title: Blog
---

The blog posts of this site are listed below, with most recent first.

 <ul>
{% assign sorted_posts = (site.categories.['blog']) %}
{% for post in sorted_posts %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
