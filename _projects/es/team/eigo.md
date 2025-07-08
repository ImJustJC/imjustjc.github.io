---
title: "EIGO"
lang: es
page_id: eigo
date: 23/09/2024
project_type: game
header_image: /assets/images/projects/eigo/eigoFront.png
featured: false
vertical_card: false
tags:
  - Godot
  - Web
---


<div class="quote-shadowbox">
Evita que La Tierra sea destruida por meteoritos mientras controlas la sobrepoblación de dinosaurios. Prueba aquí: ><a href="https://imjustjc.itch.io/eigo-earth-is-getting-overpopulated"><i class="fa-brands fa-itch-io"></i></a><
</div>
<!--content-->

<h2>Tema y la idea</h2>

<strong>EIGO: Earth is Going Overpopulated</strong> fue nuestra participación en la DinoJam 2024 como un grupo de 2 desarrolladores, usando Godot como motor gráfico. La temática de la jam era principalmente "Dinosaurios" (de ahí el nombre, claramente), pero también trajo como tema opcional "Big vs Small". Com ambas propuestas, ideamos una mecánica suficientemente simple para una jam que nos pareció entretenida y fácil de implementar.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/eigo/eigoGame1.png" style="width: 100%; margin: auto;">
</div>

Sobre el Planeta Tierra, los dinosaurios se propagan constantemente a un ritmo peligroso, pero también se enfrenta a una lluvia de meteoritos que puede destruirla por completo. Si hay demasiados dinosaurios habitando el planeta, o recibe demasiados golpes de meteorito, acabará siendo destruida. ¿La solución a ambos problemas? utilizar los dinosaurios a modo de escudo: así controlamos la población y evitamos que los meteoritos impacten.

<h2>Jugabilidad y GUI</h2>

Mi enfoque principal para el juego fue con buena parte de la jugabilidad y, sobre todo, la interfaz gráfica de usuario. Respecto a la jugabilidad, no supuso demasiado esfuerzo: el planeta rota en una dirección al pulsar "A" o "D", mientras los dinosaurios aparecen sobre su superficie. A la vez, los meteoritos que aparecen se aproximan al planeta en distintas direcciones, chocando contra lo primero que encuentren, ya sea un dinosaurio o directamente el planeta. Tras varios golpes o al alcanzar cierto número de dinosaurios con vida, la partida termina en derrota. Para la interfaz, simplemente añadí un menú de opciones con los ajustes comunes de un juego pequeño para navegador, una pantalla de estadísticas al terminar una partida, así como un menú principal con algunos detalles curiosos.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/eigo/eigoOptions.png" style="width: 48.5%; margin: auto;">
  <img src="/assets/images/projects/eigo/eigoEnd.png" style="width: 48.5%; margin: auto;">
</div>