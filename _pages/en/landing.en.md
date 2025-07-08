---
layout: single
permalink: /
lang: en
title: Home
page_id: landing
---

<style>

</style>

<div class="home_landing">
  <div class="home_about">
    <p>Hi! I'm Juan Carlos from Jaén, Andalusia, at southern Spain. Since I was little, computers always were an interest of mine, and more so videogames. That made me end up at University of Jaén studying a computer science bachelor's and master's degree, which also gave a chance on working at the computer graphics research group. Although research is not really my thing, we got some really interesting results, and even better, I managed to slip some game development in between during my free time.</p>

    <p>This website is no more than a collection of projects I've worked on, both for me as a way to remember, and for exposing my work to anyone interested (thanks for being one of them :D). As mentioned, my primary skills consist on computer graphics, specifically C++ with OpenGL and ImGUI, but I also fiddle with Unity and Godot game engines.</p>
  </div>
  <div class="home_skills">
    <h2 style="margin-top: 0.65em;">Experience</h2>
    <div style="text-align: center;">
      <h4 style="margin-top: 0.65em;">Programming</h4>
      <div style="display: flex; flex-wrap: wrap; justify-content: space-around;">
        <p class="item_box">C/C++</p>
        <p class="item_box">OpenGL</p>
        <p class="item_box">ImGUI</p>
      </div>
      <h4 style="margin-top: 0.65em;">Software</h4>
      <div style="display: flex; flex-wrap: wrap; justify-content: space-around;">
        <p class="item_box">Git</p>
        <p class="item_box">Visual Studio</p>
        <p class="item_box">Godot</p>
        <p class="item_box">Unity</p>
      </div>
    </div>
  </div>
</div>

# Featured projects

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
