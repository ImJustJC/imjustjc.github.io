---
title: "Tetris 3D"
lang: en
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
A simple 3D Tetris build with OpenGL immediate mode
</div>
<!--content-->


<video style="display: block; margin: 0 auto;" width="40%" height="auto" controls>
  <source src="/assets/videos/projects/tetris3d/tetris3dGameplay.mp4" type="video/mp4">
Sorry, video could not be loaded :(
</video>

During my Bachelor's Degree in Computer Engineering studies at University of Jaén, one of the earliest computer graphics subjects, called "Computer Graphics and Visualization", a good portion for the final score came from a final project aggregating everything learned. From the proposals given to us, I choose a 3D Tetris with basic gameplay: piece spawning and movement, scoring, and keyboard controls with some graphical user interface.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/tetris3d/tetris3DGame.png" style="width: 30%; margin: auto;">
</div>

<h2>Gameplay without a full game engine</h2>

Although Tetris mechanics are kinda simple and easy to develop, this project had to be made with OpenGL in immediate mode, the same API used during the year, with no additional libraries. It meant adding 3D models and textures by hand at a low programming level, syncing buffers and memory addresses properly, while also handling user input from system events.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/tetris3d/tetris3DUp.png" style="width: 28.5%; margin: auto;">
  <img src="/assets/images/projects/tetris3d/tetris3DSide.png" style="width: 28.5%; margin: auto;">
</div>

In its core, the game maintains a 3D matrix to simulate pieces positions; this way, I could implement piece movements over all three axis with a matrix rotation, keeping in mind collisions against game area limits. Also, I added some buttons as the GUI used to rotate the virtual camera and pausing the game to satisfy the project requirements.

<h2>3D models and textures</h2>

The main focus was to develop the game and the gameplay, but facing some extra time I opted to include a 3D model: a retro machine using lists of vertices, normals and UV, alongside a color texture. Not only the skeleton and color was added, but also some buttons and a stick at the frontal panel, giving some extra detail to the scene. Originally, my idea was to make these buttons interact and move whenever the user pressed an action, but time was short and I ended up discarding it.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/tetris3d/tetris3DRetromachine.png" style="width: 30%; margin: auto;">
</div>
