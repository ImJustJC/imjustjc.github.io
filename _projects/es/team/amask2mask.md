---
title: "A Mask 2 Mask"
lang: es
page_id: am2m
date: 1/02/2026
project_type: game
header_image: /assets/images/projects/am2m/am2mFront.png
featured: true
vertical_card: false
tags:
  - Godot
  - Web
---


<div class="quote-shadowbox">
Infiltrate entre la multitud mientras evitas ser detectado por guardias y consigues nuevas máscaras para ocultarte. Prueba aquí: ><a href="https://imjustjc.itch.io/a-mask-2-mask"><i class="fa-brands fa-itch-io"></i></a><
</div>
<!--content-->

<h2>Game Jam theme and our idea</h2>

**A Mask 2 Mask** fue nuestra participación en la primera [JaénJam](https://itch.io/jam/jaenjam-1), que propuso como temática *Mask*. Desde el primer momento, tuve la idea clara de aprovechar el doble significado del término en inglés, tanto como accesorio de disfraz como un sinónimo de ocultarse o esconderse, tomando como referencia principal las primeras entregas de la saga Assassin's Creed, donde parte del sigilo consistía en aprovechar las multitudes.

Con el poco tiempo disponible (esta JaénJam I duró solo un fin de semana) y el requerir de un ciclo desarrollo y pruebas rápido, decidimos usar Godot como herramienta principal, implementando una vista cenital y estilo pixel art, para así poder centrarnos en que el juego sea comprensible de un simple vistazo.

<h2>Jugabilidad y mecánicas</h2>

Una vez teníamos la idea clara, me encargué de implementar toda la jugabilidad, dejando a mi compañero de equipo todo el apartado visual. En primer lugar, las mecánicas de movimiento y recolecta de objetos fueron simples y asientan la base de las mecánicas principales: sigilo y detección.

El ser detectado también quedó resuelto rápidamente con raycasting, comprobando si algún guardia de seguridad tiene línea visual directa hasta el jugador, pero manejar el sigilo con las diferentes máscaras resultó ser un reto mayor. Repartidos por los niveles, distintos grupos de personajes no jugables permiten esconderte y no se detectado si equipas la misma máscara que ellos, por lo que hubo que incorporar un pequeño inventario.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/am2m/am2mLv1.png" style="width: 48.5%; margin: auto;">
  <img src="/assets/images/projects/am2m/am2mLv2.png" style="width: 48.5%; margin: auto;">
</div>

Al dejar hechas las mecánicas principales, el último punto a trabajar fue el diseño de un par de niveles para que todos los asistentes al evento pudiesen probar el juego, algo que se complicó al no tener demasiado tiempo restante (un par de horas antes de la entrega). Intenté incorporar tres niveles que fuesen escalando poco a poco en dificultad, pero finalmente solo pude añadir dos, aunque quedaron bastante bien con una buena duración. Aquí está el diseño a mano de ambos niveles, simples pero efectivos:

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/am2m/am2mDraft.jpg" style="width: 30%; margin: auto;">
</div>

<h2>El evento</h2>

Habiendo participado en varias gamejams, desde luego son un evento muy duro pero realmente gratificante. Conocer a grandes persones y ver cómo logran crear algo en tan poco tiempo es sin duda lo mejor de estos eventos, más aún cuando hay detrás un gran equipo gestionando los entresijos (¡que incluso nos regalaron varias cositas tematizadas con el evento y hubo snacks!). También llegaron a grabar y entrevistarnos a todos los participantes varias veces durante los tres días:

 - <a href="https://www.youtube.com/watch?v=GvwY-wL3-Kw">Mesón Sol <i class="fa-brands fa-youtube"></i></a>
 - <a href="https://www.youtube.com/watch?v=GofPoCvktsc">A Link to the Podcast <i class="fa-brands fa-youtube"></i></a>