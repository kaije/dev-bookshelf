---
layout: default
title: "Dev Bookshelf"
---
# Read

{% for book in site.data.books %}
  <p>
    <span class="book-title">{{ book.title }}</span><br>
    {{- book.author }}
    <br>
    <span class="reading-dates">
      {%- if book.finished -%}
        Finished {{ book.finished || date: "%e %b %Y" }}
      {%- else -%}
        Started {{ book.started || date: "%e %b %Y" -}}, still going!
      {%- endif -%}
    </span>
  </p>

<hr>
{% endfor %}