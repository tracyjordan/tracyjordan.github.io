---
layout: page
title: Blog
---

The blog posts on this site are listed below in sequence from newer to older.

 <ul>
{% assign sorted_posts = (site.categories.['blog']  | sort: 'post_date' ) %}
{% for post in sorted_posts %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
