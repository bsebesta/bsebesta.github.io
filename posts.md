---
layout: default
title: Blog
---
# {{ page.title }}

{% for post in site.posts %}
* {{ page.date | date_to_string }} :: [{{ post.title }}]({{ post.url }})
{% endfor %}
