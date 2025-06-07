---
layout: default
title: Artículos
permalink: /articulos/
---
# Artículos

<ul>
{% for articulo in site.articulos %}
  <li><a href="{{ articulo.url }}">{{ articulo.title }}</a></li>
{% endfor %}
</ul>
