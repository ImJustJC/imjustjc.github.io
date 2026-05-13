---
title: "Pylon Hodlr"
lang: en
page_id: pylonhdlr
date: 19/05/2022
project_type: game
header_image: /assets/images/projects/pylon_hodlr/pylonHodlrFront.png
featured: false
vertical_card: false
tags:
  - Unity
  - Windows
---


<div class="quote-shadowbox">
Defend your citadel from monster hordes using your special powers.
</div>
<!--content-->

<div style="width: 75%; height: auto; margin: auto; margin-bottom: 1.3rem">
  <iframe src="https://www.youtube.com/embed/mqFAkLPwb7Y" frameborder="0">
  </iframe>
</div>

<strong>Pylon Hodlr</strong> might be my favorite project made during my passing through the Bachelor's Degree in Computer Engineering, as part of the "Videogame development" subject. Being groups of 2 students, we chose things both of us liked, and ended up with something close to a RPG; out target was to add some Tower Defense mechanics, but time was short.

<h2>Characters and menu GUI</h2>

A good portion of my work in this project was focused to graphical user interface, except for the main gameplay scene: main menu, character selection and the options popup. Everything I worked on got a special care for its GUI, as I think it's one of the mandatory pillars on any kind of software.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: row;">
  <img src="/assets/images/projects/pylon_hodlr/pylonHodlrFront.png" style="width: 48.5%; margin: auto;">
  <img src="/assets/images/projects/pylon_hodlr/pylonHodlrCharacter.png" style="width: 48.5%; margin: auto;">
</div>

<strong>Pylon Hodlr</strong> was no exception; I made simple menus filled with flamboyant details. In the main menu, a background panorama replicating the classic Minecraft start screen, while at character selection an attack animation is triggered upon selecting anyone, showing a bit of the character style.

<h2>Enemy spawners</h2>

<div class="flex_image_right">
  <div style="flex: 1 1 35%">
    On the other hand, I did some work on how enemies are spawned. At the opposite side on the map, some interconnected pylons can be found, with a nexus at the center; those pylons spawn enemies around, but can be disabled by destroying them and finishing the central nexus grants the victory.
  </div>
  <div style="flex: 1 1 65%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/pylon_hodlr/pylonHodlrPylon.png" />
  </div>
</div>

The way I developed those pylons was with a 2D Delaunay triangulation to setup connections between. When a pylon is connected to a destroyed one, it starts slowly regenerating until reaching full life and becoming active again. 