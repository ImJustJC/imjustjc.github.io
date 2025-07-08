---
title: "Delaunay Interactivo"
lang: es
page_id: delaunay
date: 29/06/2022
project_type: other
header_image: /assets/images/projects/delaunay_interactive/delaunayFront.png
featured: false
vertical_card: false
tags:
  - Unity
  - Windows
---

<div class="quote-shadowbox">
Generador de triangulación de Delaunay interactiva en Unity
</div>
<!--content-->

Este proyecto corresponde a las prácticas realizadas en la asignatura "Algoritmos Geométricos" del Grado en Ingeniería Informática de la Universidad de Jaén, sirviendo como evaluación final de las mismas. El objetivo principal consiste en implementar el algoritmo de la triangulación de Delaunay en 2D, pero de forma eficiente que permita añadir interacción en tiempo real. Toda la funcionalidad que preparé para el proyecto se encuentra resumida en el siguiente vídeo: <a href="https://www.youtube.com/watch?v=M5Xa3ZU4OsU" target="_blank"><i class="fa-brands fa-youtube"></i></a>

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/delaunay_interactive/delaunayMassive.png" style="width: 100%; margin: auto;">
</div>

<h2>Interacción con el Delaunay</h2>

Además de los controles típicos para añadir o quitar puntos de la triangulación, incorporé la posibilidad de mover un punto libremente mediante el cursor. Gracias a la eficiencia del algoritmo y varias optimizaciones, la triangulación se adapta en cada fotograma al punto modificado, incluso ante situaciones críticas que provocan cambios mayores.

<div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 1.3em">
  <img style="width: 48.5%;" src="/assets/images/projects/delaunay_interactive/delaunayA.png" />
  <img style="width: 48.5%;" src="/assets/images/projects/delaunay_interactive/delaunayB.png" />
</div>

<h2>Opciones de visualización</h2>

<div class="flex_image_right">
  <p style="flex: 1 1 55%">Una propiedad de la triangulación de Delaunay es su dualidad con el diagrama de Voronoi, que también puede visualizarse a tiempo real y se ajusta a las modificaciones de forma interactiva. De igual forma, la propiedad del círculo circunscrito en cada triángulo del Delaunay también es posible visualizarla, mostrando el círculo que trazan los 3 puntos del triángulo seleccionado por el cursor.</p>
  <div style="flex: 1 1 45%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/delaunay_interactive/delaunayCircle.png">
  </div>
</div>

