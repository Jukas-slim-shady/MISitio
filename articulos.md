---
layout: default
title: Artículos
permalink: /articulos/
---

# 📰 Artículos publicados

<ul>
{% for articulo in site.articulos %}
  <li style="margin-bottom: 20px;">
    <a href="{{ articulo.url }}" style="font-weight: bold; font-size: 1.2em;">{{ articulo.title }}</a>  
    <br>
    <small>Publicado el {{ articulo.date | date: "%d/%m/%Y" }}</small>
    <p>{{ articulo.description }}</p>
  </li>
{% endfor %}
</ul>
