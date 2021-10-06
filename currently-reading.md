---
layout: default
title: "Currently reading"
---
# Currently reading

{% for book in site.data.books %}
  <p>
    <cite>{{ book.title }}</cite> by {{ book.author }}
  </p>

<hr>
{% endfor %}