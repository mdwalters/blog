---
layout: default
title: Blog Archive
---
<div class="container-fluid p-5 bg-primary text-white">
    <h1 class="display-1 text-center"><a href="/" class="text-decoration-none text-light">M.D. Walters' Blog Archives!</a></h1>
</div>

<div class="m-3">
    {% for tag in site.tags %}
        <h3>{{ tag[0] }}</h3>
        <ul>
            {% for post in tag[1] %}
                <li><a href="{{ post.url }}">{{ post.date | date: "%B %d, %Y" }} - <b>{{ post.title }}</b></a></li>
            {% endfor %}
        </ul>
    {% endfor %}
</div>
