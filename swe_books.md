---
title: Software Engineering Books
layout: default
has_children: false
---

<h1>Software Engineering Books</h1>

{% assign sorted_books = site.swe_books | sort: "rating" | reverse %}

| Title | Short |
| :---- | :------- |
{% for book in sorted_books -%}
| {{ book.title }} | {{ book.short -}} |
{% endfor -%}
