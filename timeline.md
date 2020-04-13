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
  
4

<ul>
{% assign sorted-posts = site.posts | where: %Y, 2020 | sort: 'post_date' %}
  {% for post in sorted-posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title}}</a>
  </li>
  {% endfor %}
  </ul>

  5
  
	{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}
	{% for year in postsByYear %}
	  <h3 id="{{ year.name | slugify }}">{{ year.name }}</h3>
		{% for post in year.items %}
		{% assign postYear = post.date | date:"%Y" %}
				<h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
				<h6>{{ post.author }}</h6>
			{% endfor %}
	{% endfor %}
