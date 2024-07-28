---
title: Software Engineering Books
layout: default
has_children: false
---

<h1>Software Engineering Books</h1>

{% for book in site.swe_books %}
  <h2>{{ book.title }} - {{ book.rating }}</h2>
  <p>{{ book.short | markdownify }}</p>
{% endfor %}