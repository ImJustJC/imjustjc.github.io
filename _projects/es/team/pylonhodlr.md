---
title: "Pylon Hodlr"
lang: es
page_id: pylonhdlr
date: 19/05/2022
project_type: game
header_image: /assets/images/projects/pylon_hodlr/pylonHodlrFront.png
featured: false
vertical_card: false
tags:
  - Godot
  - Web
---


<div class="quote-shadowbox">
Defiende tu ciudadela ante oleadas de monstruos con tus poderes especiales. 
</div>
<!--content-->

<div style="width: 75%; height: auto; margin: auto; margin-bottom: 1.3rem">
  <iframe src="https://www.youtube.com/embed/mqFAkLPwb7Y" frameborder="0">
  </iframe>
</div>

Uno de los proyectos que más me gustó hacer durante el Grado en Ingeniería Informática fue <strong>Pylon Hodlr</strong>, como evaluación final de la asignatura "Desarrollo de videojuegos". Siendo en grupo de 2 personas, decidimos ir un poco por algo que nos gustaba a ambos y acabamos con una especie de RPG; quisimos añadir mecánicas Tower Defense, pero no llegábamos a tiempo para la entrega.

<h2>Personajes y GUI de menús</h2>

Buena parte de mi trabajo en el proyecto esta destinado a la interfaz gráfica de usuario fuera de la escena de juego, es decir: menú principal, selección de personaje, y las opciones básicas. En todos mis desarrollos he tratado de dedicar un tiempo considerable al diseño de GUI, pues soy de los que opinan que forma el esqueleto de cualquier software.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/pylon_hodlr/pylonHodlrFront.png" style="width: 48.5%; margin: auto;">
  <img src="/assets/images/projects/pylon_hodlr/pylonHodlrCharacter.png" style="width: 48.5%; margin: auto;">
</div>

<strong>Pylon Hodlr</strong> no fue ninguna excepción; quise optar por menús muy simples pero con detalles llamativos. Para el menú principal, repliqué directamente la animación de fondo con un diorama tan típica de Minecraft, mientras que la pantalla de selección de personaje muestra una animación de ataque al seleccionar, dando una idea de la temática del personaje.

<h2>Generadores de enemigos</h2>

<div class="flex_image_right">
  <div style="flex: 1 1 35%">
    El otro aspecto que trabajé bastante es cómo aparecen los enemigos. Al extremo opuesto del mapa se encuentran una serie de pilones interconectados entre sí con un nodo en el centro; estos pilones generan enemigos, destruirlos los deshabilita y acabar con el central otorga la victoria.
  </div>
  <div style="flex: 1 1 65%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/pylon_hodlr/pylonHodlrPylon.png" />
  </div>
</div>

La forma en que implementé estos pilones utiliza una triangulación de Delaunay 2D para asignar las conexiones entre pilones. Cuando un pilón está conectado a otro que ha sido destruido, lo regenera lentamente hasta que vuelve a estar operativo. 
