<ul>
  {% for post in site.posts %}
    {%- unless post.hidden -%}
      <h2>
      <small style="color: grey;">{{ post.date | date: "%B %d, %Y at %H:%M"}}</small>
      <br>
      <a href="{{ post.url }}">{{ post.title }}</a> <small style="color: grey;">{% for tag in post.tags %}<span><b>{{ tag }} </b></span>{% endfor %}</small>
      <br>
      </h2>
    {%- endunless -%}
  {% endfor %}
</ul>
