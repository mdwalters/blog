<div class="container-fluid p-5 bg-primary text-white">
    <h1 class="display-1 text-center">M.D. Walters' Blog!</h1>
</div>

<div class="container m-3">
    {% for post in site.posts %}
        {%- unless post.hidden -%}
            <h2>
                <small>{{ post.date | date: "%B %d, %Y"}}</small>
                <br>
                <a href="{{ post.url }}">{{ post.title }}</a> <small style="color: grey;">{% for tag in post.tags %}<span><b>{{ tag }} </b></span>{% endfor %}</small>
            </h2>
        {%- endunless -%}
    {% endfor %}
    <br>
    <br>
    <h2><a href="/archive">Blog Archive</a></h2>
</div>
