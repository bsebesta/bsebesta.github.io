---
layout: default
title: Home Page
---
# {{ page.title }}

Welcome to my home page.

Here are some recent posts of mine.

{% for post in site.posts %}
* [{{ post.date | date_to_string }} :: {{ post.title }}]({{ post.url }})
{% endfor %}
