---
title: "GEU"
lang: es
page_id: geu
date: 01/01/2025
header_image: /assets/images/projects/geu/frontGEU.jpg
project_type: other
featured: false
tags:
  - Windows
  - OpenGL
  - ImGUI
---

<div class="quote-shadowbox">
Motor gráfico para nubes de puntos preparado para labores de investigación en la Universidad de Jaén.
</div>
<!--content-->

GEU (<b>G</b>eospatial and <b>E</b>nvironmental tools of <b>U</b>niversity of Jaén) es un prototipo de motor gráfico en desarrollo propiedad del <a href="https://gggj.ujaen.es/">Grupo de Gráficos y Geomática de la Universidad de Jaén</a> orientado a nubes de puntos 3D. Aunque su origen real es anterior, la aplicación utilizada en la actualidad nace hacia finales de 2021 como una plataforma en la que unificar la investigación en nubes de puntos, el punto fuerte del grupo. Viendo las necesidades y exigencias de los métodos implementados y por implementar, nos decantamos por utilizar C++ junto a OpenGL, principalmente por ser lo que estábamos aprendiendo en la carrera y su flexibilidad sin llegar a ser extremadamente complejos.

<img src="/assets/images/projects/geu/mainGEU.png" />

<h2>Interfaz gráfica de usuario</h2>

<div style="display: flex; flex-direction: row; align-items: center; margin-bottom: 1.3em; gap: 1.5em">
  <div style="flex: 1 1 50%">
      <p>
        Durante el inicio del desarrollo, tuve la oportunidad de destinar mis esfuerzos a todo lo relacionado con interfaz de usuario, tanto GUI como controles y manejo, algo que siempre me había interesado profundamente. Para facilitarnos la tarea, incluimos ImGUI como librería externa para montar una interfaz gráfica sencilla que permitiese interactuar con las funcionalidades del motor.
      </p>
      <p>
        Nuestra idea para la interfaz de usuario era clara: recrear el comportamiento de aplicaciones familiares como Unity o Blender, con un listado de objetos en la escena actual y sus detalles, además de otras ventanas para el resto de funcionalidad especializada y un control de la escena utilizando principalmente el ratón. No tardamos mucho en dar un lavado de cara al estilo visual que incluye por defecto ImGUI (imagen a la derecha), y acabamos consiguiendo una organización de ventanas y paleta de color que continúa usandose a día de hoy (imagen del inicio).
      </p>
  </div>
  <div style="flex: 1 1 50%">
    <img src="/assets/images/projects/geu/oldGEU.png" />
  </div>
</div>

<h2>Mis aportes a GEU</h2>

Aunque mi enfoque principal es la interfaz de usuario, también trabajé en otros aspectos de GEU más específicos; realmente, la aplicación estaba suficientemente preparada para su uso al cabo de un año o algo más, y el grupo necesitaba un flujo constante de trabajos de investigación.

<h3>Artículos científicos</h3>

<ul>
  <li>
    <a href="https://diglib.eg.org/items/eab6a149-f1e2-4726-9a14-3a27e29ffd6e">An Efficient Point Selection Process over a Meshlet-structured Point Cloud</a>: Durante 2023 recibí la propuesta de publicar un póster al Congreso Español de Informática Gráfica de 2024, en el que destacaría los avances que realicé sobre GEU en cuanto a selección de puntos. Como pequeño resumen, GEU implementa un sistema de optimización que agrupa conjuntos de puntos para mejorar el rendimiento del renderizado (<a href="https://developer.nvidia.com/blog/introduction-turing-mesh-shaders/"><i>meshlets</i></a>), con una estructura de datos organizada para la tarjeta gráfica. Aprovechando esta estructura, el proceso de selección de puntos también	puede mejorarse considerablemente, aunque no tanto como mantener otras estructuras espaciales pero lo suficiente como para no requerir estructuras adicionales. Lo que originalmente estaba pensado como póster acabó tornando a un trabajo corto y una ponencia en el congreso, que se celebró en Galicia y al que pude asistir presencialmente.
  </li>
  <li>
    <a href="https://www.sciencedirect.com/science/article/pii/S016816992500208X">Meshlets based data model for real-time interaction and analysis with hyper-spectral vegetation data</a>: Una vez presentado mi primer artículo, no tardó en llegar una propuesta para el siguiente, esta vez un trabajo científico destinado a revista. Siguiendo con los mismos conceptos, exploramos la utilidad de la estructura interna que implementa GEU, y dimos con un método para optimizar el almacenamiento y uso de ingentes cantidades de datos sobre las nubes de puntos, con unos resultados muy prometedores. Todo el contenido quedó implementado directamente en GEU, demostrando la flexibilidad de la aplicación y habilitando que el resto de miembros del grupo puedan acceder a esta utilidad. 
  </li>
</ul>

