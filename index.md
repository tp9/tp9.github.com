---
layout: page
title: Latest threads
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts limit:4 %}
<span><h1>{{ post.date | date: '%B' }} {{ post.date | date: '%e' }}, {{ post.date | date: '%Y' }}</h1></span>
<p>
    {{ post.content }}
</p>
{% endfor %}
