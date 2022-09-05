<ul>
  {% for post in site.posts %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a>
    
    <small>{{ post.teaser }}</small>
    </h3>
      


  {% endfor %}
</ul>
