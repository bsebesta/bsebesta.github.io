---
layout: default
title: Books
---
{% assign booklist = site.data.books | sort: 'author' %}
# {{ page.title }}

I love books! Let me tell you about some.

{% for entry in site.data.books %}
* **{{ entry.book_name }}** by _{{ entry.author }}_
{% endfor %}
