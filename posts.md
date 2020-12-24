---
layout: default
title: Posts
---
# {{ page.title }}

<ul>
{% for post in site.posts %}
<li style="margin: .3rem 0;"><span style="background-color: hsl(0,0%,90%); padding: .1rem; border-radius: 3px;">{{ post.layout }}</span> <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>