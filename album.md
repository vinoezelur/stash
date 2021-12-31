---
layout: default
title: .pics
---
<h1>Pics Pics and more Pics</h1>

<ul>
    {% for album in site.albums %}
    <li>
        <h2><a href="{{ album.url }}">{{ album.name }}</a></h2>
        <h3>{{ album.location }}</h3>
        <p>{{ album.content | markdownify }}</p>
    </li>
    {% endfor %}
</ul>