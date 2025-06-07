---
layout: default
title: Inicio
---

# Bienvenido a mi sitio web

Este sitio fue creado como parte de un examen práctico utilizando **GitHub Pages** y **Jekyll**.

---

## 📄 Secciones principales

- [Acerca de](about)
- [Contacto](contact)
- [Artículos](articulos)

---

## 📰 Últimos artículos

<ul>
{% for articulo in site.articulos limit:2 %}
  <li>
    <a href="{{ articulo.url }}">{{ articulo.title }}</a>
  </li>
{% endfor %}
</ul>

---

## 📷 Imagen opcional

![Ejemplo de imagen](https://via.placeholder.com/600x200?text=Bienvenido+al+sitio)
