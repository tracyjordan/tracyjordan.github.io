---
layout: page
title: Categories
---

The posts on this site are in categories and listed below in sequence from newer to older.

<h2>Aroha.dev</h2>

{% assign postsByYear = (site.categories.['aroha'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>{{ year.name }}</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

<h2>Art</h2>

{% assign postsByYear = (site.categories.['art'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>{{ year.name }}</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}
