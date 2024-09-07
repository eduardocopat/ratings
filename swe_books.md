---
title: Software Engineering Books
layout: default
has_children: false
---

 <style>
        .gray-paragraph {
            color: #A9A9A9;
        }
    </style>

<h1>Software Engineering Books</h1>

The books that impacted my career the most. 

Sorted by tier and alphabetically. Books are dated after their first release.

{% assign sorted_books = site.swe_books | sort: "title"  %}
<h2>S Tier — Quintessential for every software engineer </h2>
{% for book in sorted_books %}
{% if book.rating == "S-Tier" %}
- **{{ book.title }}** _({{ book.year }}) - {{ book.author }}_ <br>
{{ book.short}}
{% endif %}
{% endfor %}


<h2>A+ Tier — Highly recommended books</h2>
{% for book in sorted_books %}
{% if book.rating == "A+-Tier" %}
- **{{ book.title }}** _({{ book.year }}) - {{ book.author }}_ <br>
{{ book.short}}
{% endif %}
{% endfor %}

<h2>A Tier — Good references</h2>
{% for book in sorted_books %}
{% if book.rating == "A-Tier" %}
- **{{ book.title }}** _({{ book.year }}) - {{ book.author }}_ <br>
{{ book.short}}
{% endif %}
{% endfor %}

<h2>B Tier — Interesting</h2>
{% for book in sorted_books %}
{% if book.rating == "B-Tier" %}
- **{{ book.title }}** _({{ book.year }}) - {{ book.author }}_ <br>
{{ book.short}}
{% endif %}
{% endfor %}

<h2>C Tier — Don't even</h2>