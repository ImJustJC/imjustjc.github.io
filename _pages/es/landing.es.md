---
layout: single
permalink: /
lang: es
title: Inicio
page_id: landing
---

<div class="home_landing">
  <div class="home_about">
    <p>¡Hola! Soy Juan Carlos y te doy la bienvenida a mi pequeño rincón personal :). Desde pequeño, siempre me interesaron los ordenadores en general, y especialmente los videojuegos. De ahí que acabase en la Universidad de Jaén estudiando el grado y máster en Ingeniería Informática, consiguiendo además la oportunidad de trabajar en el grupo de investigación de informática gráfica. Aunque la investigación no es mi punto fuerte, conseguimos resultados muy prometedores, e incluso pude encajar un poco de desarrollo de videojuegos en mi tiempo libre.
    </p>
    <p>Esta web la enfoco como una colección de los proyectos en los que he trabajado, sirviendo para mí como una forma de recordar, y como método para exponer mis proyectos con cualquier interesado (gracias por ser uno de ellos :D). En resumen, mis aptitudes principales se centran en la informática gráfica, especialmente C++, OpenGL e ImGUI, aunque también he trasteado con los motores gráficos Unity y Godot.
    </p>
  </div>
  <div class="home_skills">
    <h2 style="margin-top: 0.65em;">Experiencia</h2>
    <div style="text-align: center;">
      <h4 style="margin-top: 0.65em;">Programación</h4>
      <div style="display: flex; flex-wrap: wrap; justify-content: space-around;">
        <p class="item_box">C/C++</p>
        <p class="item_box">OpenGL</p>
        <p class="item_box">ImGUI</p>
      </div>
      <h4 style="margin-top: 0.65em;">Software</h4>
      <div style="display: flex; flex-wrap: wrap; justify-content: space-around;">
        <p class="item_box">Git</p>
        <p class="item_box">Visual Studio</p>
        <p class="item_box">Godot</p>
        <p class="item_box">Unity</p>
      </div>
    </div>
  </div>
</div>

# Proyectos destacados

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>