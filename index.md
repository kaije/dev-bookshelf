---
layout: default
title: "Dev Bookshelf"
---
# Read in 2021

{% for book in site.data.books %}
  <p>
    <cite>{{ book.title }}</cite> by {{ book.author }}
    <br>
    <span>
    Started {{ book.started }}
    {% if book.finished %}    
    , finished {{ book.finished }}
    {% else %}
    , still going
    {% end if %}
    </span>
  </p>

<hr>
{% endfor %}