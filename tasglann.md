---
layout: page
title: Tasglann
permalink: /tasglann/
---

<div class="list-group">

{% for post in site.posts %}
	{% assign currentDate = post.date | date: "%Y" %}
	{% if currentDate != myDate %}
		<h2 class="archive-page-date">{{ currentDate }}</h2>
		{% assign myDate = currentDate %}
	{% endif %}
	<a class="list-group-item list-group-item-action" href="{{ site.baseurl }}{{ post.url }}">
	<div class="col-4">
		<span>{{ post.date | date: "%Y-%m-%d" }}</span> &nbsp; &nbsp;
		</div>
		<div class="col-8">
		{{ post.title }}
		</div>
	</a>
{% endfor %}

</div>
