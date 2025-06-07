---
layout: default
title: Inicio
---

<section style="text-align:center; margin: 40px 0;">
  <h1>Bienvenido a Sitio de Examen</h1>
  <p>Un espacio creado con Jekyll para demostrar tus habilidades en desarrollo web y gestión de contenido.</p>
</section>

<section style="margin: 30px 0;">
  <h2>Nuestros Artículos Destacados</h2>
  <p>Explora algunos de nuestros artículos más recientes y populares:</p>
  <ul>
    {% for articulo in site.articulos limit:3 %}
      <li>
        <a href="{{ articulo.url }}">{{ articulo.title }}</a>  
        <br>
        <small>Publicado el {{ articulo.date | date: "%d/%m/%Y" }}</small>
        <p>{{ articulo.description }}</p>
      </li>
    {% endfor %}
  </ul>
</section>

<section style="margin: 30px 0;">
  <h2>Sobre este sitio</h2>
  <p>Este sitio fue creado para cumplir con los requisitos del examen práctico, usando Jekyll y GitHub Pages.</p>
  <p>Aquí puedes encontrar artículos interesantes, información de contacto y más.</p>
</section>

<section style="margin: 30px 0;">
  <h2>Contáctanos</h2>
  <p>¿Tienes dudas o quieres más información? Visita la página de contacto para enviarnos un mensaje.</p>
  <p><a href="/contact.html">Ir a Contacto</a></p>
</section>
