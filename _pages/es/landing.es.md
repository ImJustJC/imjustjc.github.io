---
layout: single
permalink: /
lang: es
title: Inicio
page_id: landing
---

¡Hola! Soy Juan Carlos, aunque quienes me han sufrido me llaman directamente JC, y desde 2020 o por ahí me gusta intentar hacer juegos. Estudié grado y máster de Ingeniería Informática en la Universidad de Jaén y en los pocos ratos libres que tenía fuí probando a desarrollar alguna idea con motores gráficos varios. Actualmente trabajo con el Grupo de Gráficos y Geomática de la UJA desde hace un par de años ya y he publicado con ellos dos artículos científicos. Visita mi página de LinkedIn (al pie de cualquier página en todo momento, pero te lo dejo aquí tambien esta vez <a href="https://www.linkedin.com/in/juan-carlos-fernández-pérez-462622220/"><i class="fa-brands fa-linkedin"></i></a>) para más detalles sobre mi vida estudiantil y profesional, este espacio lo reservo para mis jueguicos :D

# Proyectos destacados

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
