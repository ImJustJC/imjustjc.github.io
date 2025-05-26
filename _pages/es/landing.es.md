---
layout: single
permalink: /
lang: es
title: Inicio
page_id: landing
---

<div style="display: flex; flex-direction: column; gap: 1.3rem;">
  <div>
    <p>
      ¡Hola! Soy Juan Carlos, aunque quienes me han sufrido me llaman directamente JC, y desde 2020 o por ahí me gusta
      intentar hacer juegos. Estudié grado y máster de Ingeniería Informática en la Universidad de Jaén y en los pocos
      ratos libres que tenía iba probando a desarrollar alguna idea con motores gráficos varios, pero ahora mismo estoy
      enamorado de ✨Godot✨ y tengo un poco (bastante) rencor a Unity >:(
    </p>
  </div>
  <div style="display: flex; flex-direction: column; align-items: center;">
    <iframe
      src="https://gamer2810.github.io/steam-miniprofile/?accountId=76561198095287506&lang=spanish&appId=367520&interactive=true&vanityId=ImJustJC"
      name="steamMiniProfilePreview" scrolling="no" frameborder="0" allowfullscreen="false"
      style="border:0px #ffffff none;" name="myiFrame" scrolling="no" frameborder="1" marginheight="0px"
      marginwidth="0px" height="300px" width="320px" allowfullscreen></iframe>
    <a href="https://backloggd.com/u/ImJustJC/" style="display: block; margin: auto;">Backloggd - ImJustJC</a>
  </div>
</div>


# Proyectos destacados

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>