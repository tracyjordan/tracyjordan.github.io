---
layout: page
title: Categories
---

The posts on this site are in categories and listed below in sequence from newer to older.

{% assign postsByYear = (site.categories.['art'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Art ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['books'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Books ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['māori'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Māori ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}


{% assign postsByYear = (site.categories.['meditation'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Meditation ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['podcasts'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Podcasts ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['poetry'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Poetry ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['professional'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Professional ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['terminology'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Terminology ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['therapy'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Therapy ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}

{% assign postsByYear = (site.categories.['walks'] | group_by_exp:"post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}
<h2>Walks ({{ year.name }})</h2>
<ul>
{% for post in year.items %}
{% assign postYear = post.date | date:"%Y" %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>		
{% endfor %}
</ul>	
{% endfor %}
