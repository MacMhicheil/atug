---
layout: page
title: Tasglann
permalink: /tasglann/
---

{% for post in site.posts %}
	{% assign currentDate = post.date | date: "%Y" %}
	{% if currentDate != myDate %}
		<h2 class="archive-page-date">{{ currentDate }}</h2>
		{% assign myDate = currentDate %}
	{% endif %}
	<a href="{{ site.baseurl }}{{ post.url }}">
			{{ post.date | date: "%Y-%m-%d" }} &nbsp; &nbsp; {{ post.title }}
	</a>
{% endfor %}
