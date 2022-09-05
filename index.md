<ul>
  {% for post in site.posts %}
    <h3>
    <small style="color: grey;">{{ post.date | date: "%B %d, %Y"}}</small>
    <br>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <br>
    {%- if post.teaser -%}
      <small>{{ post.teaser }}</small>
    {%- endif -%}
    </h3>
  {% endfor %}
</ul>
