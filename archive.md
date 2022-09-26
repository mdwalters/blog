---
layout: default
title: Blog Archive
---
{% for tag in site.tags %}
  {%- unless post.hidden -%}
    <h3>{{ tag[0] }}</h3>
    <ul>
      {% for post in tag[1] %}
        <li><a href="{{ post.url }}">{{ post.date | date: "%B %d, %Y at %H:%M" }} - <b>{{ post.title }}</b></a></li>
      {% endfor %}
    </ul>
  {%- endunless -%}
{% endfor %}
