---
layout: default
title: Reading
---
{% assign booklist = site.data.books | sort: 'author' %}
# {{ page.title }}

I love books! 

## 2021

<ul>
{% for book in site.books %}
<li style="margin: .3rem 0;"><span style="background-color: hsl(0,0%,90%); padding: .1rem; border-radius: 3px;">{{ book.category }}</span> <a href="{{ book.url }}">{{ book.title }}</a></li>
{% endfor %}
</uL>

## 2020

<ul>
{% assign books_2020 = site.data.books | where: "year","2020" %}
{% for book in books_2020 %}
<li style="margin: .3rem 0;"><span style="font-weight: 700">{{ book.book_name }}</span> by <em>{{ book.author }}</em></li>
{% endfor %}
</uL>

## 2019

<ul>
{% assign books_2020 = site.data.books | where: "year","2019" %}
{% for book in books_2020 %}
<li style="margin: .3rem 0;"><span style="font-weight: 700">{{ book.book_name }}</span> by <em>{{ book.author }}</em></li>
{% endfor %}
</uL>

<!--
{% for entry in site.data.books %}
* **{{ entry.book_name }}** by _{{ entry.author }}_
{% endfor %}
-->