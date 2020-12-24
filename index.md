---
layout: default
title: Home Page
---
# About Me
My name is Bryan Sebesta. I'm a UX designer working at [RAIN Agency](http://www.rain.agency). I'm looking forward to this pandemic ending.

This is my little corner of the internet. A digital garden, blog, and site for experimentation, where I can design, code, write, and experiment with freedom.

If you want to reach me, you can:
* [Email me](mailto:hello@bryansebesta.com)
* Check out [my LinkedIn](https://www.linkedin.com/in/bryansebesta/)

## Recent Posts

{% assign fp_posts = site.posts | where:"fp_visibility","true" %}
<ul>
{% for post in fp_posts limit:3 %}
<li style="margin: .3rem 0;"><span style="background-color: hsl(0,0%,90%); padding: .1rem; border-radius: 3px;">{{ post.layout }}</span> <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

## Contact me