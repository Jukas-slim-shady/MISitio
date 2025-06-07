---
layout: default
title: Artículos
permalink: /articulos/
---

# 📰 Artículos publicados

A continuación encontrarás una lista de artículos creados como parte del proyecto. Están organizados en una colección y se generan automáticamente con Jekyll.

---

{% for articulo in site.articulos %}
<div style="border-bottom: 1px solid #ddd; padding: 1em 0;">
  <h3 style="margin-bottom: 0;"><a href="{{ articulo.url }}">{{ articulo.title }}</a></h3>
  <small>Publicado el {{ articulo.date | date: "%d/%m/%Y" }}</small>
  <p>{{ articulo.description }}</p>
</div>
{% endfor %}
