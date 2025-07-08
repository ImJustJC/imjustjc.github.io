---
title: "Beat Heisters"
lang: es
page_id: beatheisters
date: 31/05/2021
project_type: game
header_image: /assets/images/projects/beat_heisters/beatHeistersFront.png
featured: false
vertical_card: false
tags:
  - Unity
  - Windows
---


<div class="quote-shadowbox">
Aguanta tu posición tras robar un banco siguiendo el ritmo de la música.
</div>
<!--content-->

<video style="display: block; margin: 0 auto;" width="75%" height="auto" controls>
  <source src="/assets/videos/projects/beat_heisters/beat_heisters_gameplay.mp4" type="video/mp4">
Vaya, no se ha podido cargar el vídeo :(
</video>

Como parte de mis estudios del Grado en Ingeniería Informática en la Universidad de Jaén, una de las asignaturas se dedica a una introducción a las tecnologías multimedia, llamada "Sistemas Multimedia", en la que se presenta el funcionamiento de la codificación para formatos de imagen, video y audio más comunes. A modo de proyecto de prácticas, nos juntamos 2 personas para hacer un prototipo de juego de ritmo.

<h2>Jugabilidad en tercera persona</h2>

<div class="flex_image_right">
  <div style="flex: 1 1 35%">
    <p>
      El juego en sí no es nada complejo, aunque cuenta con varias mecánicas interesantes. El objetivo principal es aguantar en un banco recién robado, manteniendo tu posición contra la policía utilizando tres armas distintas:
    </p>
    <ul>
      <li><strong>Rifle de asalto</strong>: Arma principal, dispara una bala en cada golpe del ritmo detectado.</li>
      <li><strong>Escudo</strong>: Bloquea los disparos recibidos de frente, pero solo se activa al golpe del ritmo.</li>
      <li><strong>Granada</strong>: Lanza una granada al ritmo con un tiempo considerable de reutilización que puede acabar con varios enemigos.</li>
    </ul>    
  </div>
  <div style="flex: 1 1 65%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/beat_heisters/beatHeistersStoreroom.png" />
  </div>
</div>


<h2>Lo interesante: detección del <i>onset</i></h2>

Realmente, nuestro esfuerzo quedó centralizado en un sistema capaz de detectar el "pulso" de una pista de audio cualquiera. Un sistema así no es tarea fácil con el amplio abanico de estilos musicales y la infinidad de interpretaciones por cada artista, pero siempre pueden intentar extraerse algunos patrones genéricos.


<div class="flex_image_right">
  <div style="flex: 1 1 60%">
      <p>
        Cualquier obra musical sigue un ritmo definido como un sonido repetitivo y espaciado equitativamente durante toda la pista; esto es lo que nuestro sistema busca para definir cuándo ocurre una acción en el juego. Mientras se reproduce la música de fondo, se realiza un análisis interno de la frecuencia que marca la señal de audio, generando una curva con diferentes picos de amplitud en aquellos instantes donde suene una nota más marcada que el resto.
      </p>
  </div>
  <div style="flex: 1 1 40%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/beat_heisters/onsetCurve.png" />
  </div>
</div>

A partir de esta curva, la implementación que realizamos aplica una normalización utilizando una ventana local cercana a cada instante en el tiempo, marcando más los picos de la curva. Tras filtrar y mantener solo los picos más altos y que se repiten a intervalos similares, tenemos una aproximación del <i>tempo</i> de la pista musical.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/beat_heisters/onsetCurveNormalized.png" style="width: 60%; margin: auto;">
</div>
