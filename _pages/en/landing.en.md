---
layout: single
permalink: /
lang: en
title: Home
page_id: landing
---

<div class="home_about">
  <div>
    <p>
      Hi there! I'm Juan Carlos, but everyone ends up calling me JC, and I fiddling with making games around 2020. I studied a Computer Engineering bachelor's and master's degree at University of Jaén (UJA), taking any tiny free time I had trying to develop some game ideas with a any game engine I could find. Currently in love with ✨Godot✨ and kind of hating Unity >:(
    </p>
  </div>
  <div>
    <iframe
      src="https://gamer2810.github.io/steam-miniprofile/?accountId=76561198095287506&appId=367520&interactive=true&vanityId=ImJustJC"
      name="steamMiniProfilePreview" scrolling="no" frameborder="0" allowfullscreen="false"
      style="border:0px #ffffff none;" name="myiFrame" scrolling="no" frameborder="1" marginheight="0px"
      marginwidth="0px" height="300px" width="320px" allowfullscreen></iframe>
  </div>
</div>

# Featured projects

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
