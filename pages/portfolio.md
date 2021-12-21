---
layout: page
title: Porfatolio
permalink: /portfolio
---
<ul>
{% for product in site.portfolio %}
    <li>
        Título: {{ product.title }} | Contenido: {{ product.content | remove: '<p>' | remove: '</p>' | truncate: 40 }}
        <br>
        <a href="{{ product.url }}">{{ product.title }}</a>
    </li>
{% endfor %}
</ul>
