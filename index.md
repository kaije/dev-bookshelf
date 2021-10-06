---
layout: default
title: "Dev Bookshelf"
---
# Read

{% for book in site.data.books %}
  <p>
    <cite>{{ book.title }}</cite> by {{ book.author }}
    <br>
    <span class="reading-dates">
      Started {{ book.started || date: "%e %b" -}}
      {%- if book.finished -%}
        , finished {{ book.finished || date: "%e %b %Y" }}
      {%- else -%}
        , still going!
      {%- endif -%}
    </span>
  </p>

<hr>
{% endfor %}