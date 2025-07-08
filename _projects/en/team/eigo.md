---
title: "EIGO"
lang: en
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
Take care of Earth by blocking incoming meteors while you manage dinosaur population. Try it here: ><a href="https://imjustjc.itch.io/eigo-earth-is-getting-overpopulated"><i class="fa-brands fa-itch-io"></i></a><
</div>
<!--content-->

<h2>The theme and the idea</h2>

<strong>EIGO: Earth is Going Overpopulated</strong> was our entry to DinoJam 2024 as a two person team, using Godot as the game engine. The jam's main theme was, obviously, "Dinosaurs", but it brought the additional theme "Big vs Small". With both themes, we came up with a simple enough gameplay mechanic for a jam that looked engaging and easy to develop.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/eigo/eigoGame1.png" style="width: 100%; margin: auto;">
</div>

Over Planet Earth, dinosaurs proliferate dangerously, while a meteor shower endangers the planet safety. If many dinosaurs populate Earth, or it gets hit many times by meteors, it will be destroyed. How to solve both problems? using dinosaurs as the shield: we can handle population and prevent meteor impacts.

<h2>Gameplay and GUI</h2>

I mainly focused on gameplay and graphical user interface during development. Gameplay mechanics didn't pose a challenge: the planet rotates in a direction when "A" or "D" is pressed, with dinosaurs appearing randomly over the surface. At the same time, meteors spawn and target Earth from any direction, crashing with anything they touch, be it a dinosaur or the planet. After being hit many times or reaching a high count of dinosaurs alive at any moment, the game ends. For the GUI, I just added a common options menu, a statistics screen at the end of a game, and a main menu containing some funny little things.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/eigo/eigoOptions.png" style="width: 48.5%; margin: auto;">
  <img src="/assets/images/projects/eigo/eigoEnd.png" style="width: 48.5%; margin: auto;">
</div>