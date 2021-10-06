---
layout: default
title: "Dev Bookshelf"
---
# Read in 2021

{% for book in site.data.books %}
  <p>
    <cite>{{ book.title }}</cite> by {{ book.author }}
  </p>

<hr>
{% endfor %}