<ul>
  {% for post in site.posts %}
    <h3>
    <a href="{{ post.url }}">{{ post.title }}</a> <small style="color: grey;">{% for tag in page.tags %}<span>{{ tag }} </span>{% endfor %}</small>
    <br>
    <small>{{ post.teaser }}</small>
    </h3>
    <br><br>
  {% endfor %}
</ul>
