---
title: "GEU"
lang: es
page_id: geu
date: 30/06/2025
header_image: /assets/images/projects/geu/frontGEU.jpg
project_type: other
featured: true
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

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/geu/mainGEU.png" style="width: 100%; margin: auto;">
</div>

<h2>Interfaz gráfica de usuario</h2>

<div style="align-items: center; margin-bottom: 1.3em; gap: 1.5em">
  <p>
    Durante el inicio del desarrollo, tuve la oportunidad de destinar mis esfuerzos a todo lo relacionado con interfaz de usuario, tanto GUI como controles y manejo, algo que siempre me había interesado profundamente. Para facilitarnos la tarea, incluimos ImGUI como librería externa para montar una interfaz gráfica sencilla que permitiese interactuar con las funcionalidades del motor.
  </p>
  <p>
    Nuestra idea para la interfaz de usuario era clara: recrear el comportamiento de aplicaciones familiares como Unity o Blender, con un listado de objetos en la escena actual y sus detalles, además de otras ventanas para el resto de funcionalidad especializada y un control de la escena utilizando principalmente el ratón. No tardamos mucho en dar un lavado de cara al estilo visual que incluye por defecto ImGUI, y acabamos consiguiendo una organización de ventanas y paleta de color que continúa usándose a día de hoy.
  </p>
</div>

<div style="display: grid; grid-template-columns: repeat(2, 1fr); justify-items: center; column-gap: 1.3rem;">
  <p><strong>Captura de pantalla de la versión actual de GEU</strong></p>
  <p><strong>Captura de pantalla de la versión original de GEU</strong></p>
  <img src="/assets/images/projects/geu/hyperGEU.png" alt="Captura de pantalla de la versión actual de GEU">
  <img src="/assets/images/projects/geu/oldGEU.png" alt="Captura de pantalla de la versión original de GEU">
</div>


<h2>Funcionalidad modular</h2>

<div class="flex_image_right">
  <div style="flex: 1 1 55%">
      <p>
        Además del uso para renderizado, GEU necesitaba una gestión precisa de datos espectrales y su análisis, el enfoque principal del grupo de investigación. Esta funcionalidad adicional no se emparejaba del todo con las cosas de motor gráfico y están desarrolladas por otros miembros, por lo que se diseñó un sistema de módulo que permitiese encapsular funcionalidad específica y aislarla del resto de la aplicación.
      </p>
      <p>
        Al principio, estos módulos se añadían directamente al proyecto, pero no tardó en generar problemas de escala a medida que más desarrolladores se unían al grupo. Con ello, empecé a trabajar en un rediseño por completo del sistema de módulos, utilizando un enfoque dinámico en su lugar: en vez de cargar todos los módulos al inicio, el usuario selecciona qué modulo añadir mientras se ejecuta GEU. Este sistema se implementa mediante librerías de vinculación dinámica (DLL) en Windows, y ha resultado ser un añadido de gran utilidad para usuarios y otros desarrolladores.
      </p>
  </div>
  <div style="flex: 1 1 45%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/geu/modulesGEU.png" />
  </div>
</div>

<h2>Escaneo espectral y fusión de datos</h2>

Construir un motor gráfico, aunque útil, no era suficiente para el grupo de investigación. Debía añadirse mucha funcionalidad específica, resultando en la implementación del sistema de módulos. Desde entonces, GEU ha recibido bastantes módulos, pero la fusión de datos siempre ha sido esencial y la primera categoría implementada. La fusión de datos significa combinar los conjuntos de datos espectrales y espaciales; esto es, tomar un conjunto de datos espectrales y una nube de puntos escaneada, asignando los valores espectrales correspondientes a cada punto de la nube.

Nuestro trabajo incluía tres tipos de sensores espectrales: térmico, multiespectral e <strong>hiperespectral</strong>. En mi caso, acabé encargado de la fusión hiperespectral, un gran reto dada la magnitud de los datos que emplea, forzando el uso de múltiples optimizaciones para asegurar un buen rendimiento. A la vez, esta fusión formó el punto de entrada a un módulo de análisis así como varias oportunidades de redactar un artículo científico. La siguiente imagen muestra un resumen de esto último, presentando la signatura hiperespectral de un área seleccionada empleando los datos reales (gráfica naranja) contra los datos de nuestro sistema (gráfica azul), que han sido agregados y simplificados para un uso mucho más eficiente:

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/geu/hyperDataGEU.png" style="width: 100%; margin: auto;">
</div>


<h2>Mis aportes a GEU</h2>

Entre todo el trabajo que realicé en GEU, también pude publicar algunos artículos científicos en esos años:

<h3>Artículos científicos</h3>

<ul>
  <li>
    <a href="https://diglib.eg.org/items/eab6a149-f1e2-4726-9a14-3a27e29ffd6e">An Efficient Point Selection Process over a Meshlet-structured Point Cloud</a>: Durante 2023 recibí la propuesta de publicar un póster al Congreso Español de Informática Gráfica de 2024, en el que destacaría los avances que realicé sobre GEU en cuanto a selección de puntos. Como pequeño resumen, GEU implementa un sistema de optimización que agrupa conjuntos de puntos para mejorar el rendimiento del renderizado (<a href="https://developer.nvidia.com/blog/introduction-turing-mesh-shaders/"><i>meshlets</i></a>), con una estructura de datos organizada para la tarjeta gráfica. Aprovechando esta estructura, el proceso de selección de puntos también	puede mejorarse considerablemente, aunque no tanto como mantener otras estructuras espaciales pero lo suficiente como para no requerir estructuras adicionales. Lo que originalmente estaba pensado como póster acabó tornando a un trabajo corto y una ponencia en el congreso, que se celebró en Galicia y al que pude asistir presencialmente.
  </li>
  <li>
    <a href="https://www.sciencedirect.com/science/article/pii/S016816992500208X">Meshlets based data model for real-time interaction and analysis with hyper-spectral vegetation data</a>: Una vez presentado mi primer artículo, no tardó en llegar una propuesta para el siguiente, esta vez un trabajo científico destinado a revista. Siguiendo con los mismos conceptos, exploramos la utilidad de la estructura interna que implementa GEU, y dimos con un método para optimizar el almacenamiento y uso de ingentes cantidades de datos sobre las nubes de puntos, con unos resultados muy prometedores. Todo el contenido quedó implementado directamente en GEU, demostrando la flexibilidad de la aplicación y habilitando que el resto de miembros del grupo puedan acceder a esta utilidad. 
  </li>
</ul>

