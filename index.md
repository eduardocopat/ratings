---
title: Home
layout: home
---
Personal ratings on media.

<ul>
  {% for page in site.pages %}
     {% if page.title and page.url != "/" and page.url != "/404.html" %}
      <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>