---
title: "Tetris 3D"
lang: es
page_id: tetris3d
date: 06/01/2021
project_type: game
header_image: /assets/images/projects/tetris3d/tetris3DFront.png
featured: false
vertical_card: true
tags:
  - OpenGL
  - Windows
---

<div class="quote-shadowbox">
Un simple Tetris en 3D implementado con OpenGL en modo inmediato
</div>
<!--content-->

<video style="display: block; margin: 0 auto;" width="40%" height="auto" controls>
  <source src="/assets/videos/projects/tetris3d/tetris3dGameplay.mp4" type="video/mp4">
Vaya, no se ha podido cargar el vídeo :(
</video>

Como parte de mis estudios del Grado en Ingeniería Informática en la Universidad de Jaén, durante una de las primeras asignaturas dedicadas al informática gráfica, "Informática Gráfica y Visualización", parte de la calificación final se ligaba a un proyecto final que agregase todo lo aprendido. Entre las múltiples propuestas, elegí implementar un Tetris en 3D con su jugabilidad básica: generación y movimiento de piezas, puntuación y controles con teclado y en pantalla.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/tetris3d/tetris3DGame.png" style="width: 30%; margin: auto;">
</div>

<h2>Jugabilidad sin motor gráfico</h2>

Si bien las mecánicas más simples de Tetris son simples de implementar, el proyecto debía realizarse utilizando OpenGL en modo inmediato, la API que aprendimos durante el curso, sin incorporar librerías adicionales. Esto supone incorporar los modelos y texturas manualmente a bajo nivel, asignando búferes y direcciones de memoria con precisión, así como gestionar la interacción a partir de los eventos de entrada.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/tetris3d/tetris3DUp.png" style="width: 28.5%; margin: auto;">
  <img src="/assets/images/projects/tetris3d/tetris3DSide.png" style="width: 28.5%; margin: auto;">
</div>

Internamente, el juego se mantiene sobre una matriz 3D, donde cada celda corresponde a un bloque del área de juego; así, pude definir los movimientos de cada pieza sobre los tres ejes como rotaciones de la matriz, e incluso controlar el choque contra los límites del área. También incluí algunos botones en la interfaz gráfica para rotar la cámara y pausar el juego para cumplir con los requisitos del proyecto.

<h2>Modelados y texturas</h2>

Aunque lo principal es el juego y sus controles, decidí incorporar algo más mediante un modelo 3D, una máquina recreativa asignada a mano mediante un listado de vértices, normales y UV, junto a una textura que añada el color. No solo me propuse hacer el esqueleto de la máquina, también añadí algunos botones y una palanca en el panel frontal, detallando un poco más la escena. Mi idea original fue que estos botones y la palanca se activasen y moviesen cuando el jugador estaba jugando, pero el tiempo era limitado y decidí descartarlo finalmente.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/tetris3d/tetris3DRetromachine.png" style="width: 30%; margin: auto;">
</div>