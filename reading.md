---
layout: default
title: Reading
---
{% assign booklist = site.data.books | sort: 'author' %}
# {{ page.title }}

I love books! Let me tell you about some.

{% for book in site.books %}
* {{ book.title }}
{% endfor %}

<!--
{% for entry in site.data.books %}
* **{{ entry.book_name }}** by _{{ entry.author }}_
{% endfor %}
-->