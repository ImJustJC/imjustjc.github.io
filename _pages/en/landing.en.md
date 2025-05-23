---
layout: single
permalink: /
lang: en
title: Home
page_id: landing
---


<div style="display: flex; gap: 1.3rem;">
  <div>
    <p>
      Hi there! I'm Juan Carlos, but everyone ends up calling me JC, and I started making games around 2020. I studied a bachelor's and master's degree at University of Jaén (UJA), taking any tiny free time I had trying to develop some game ideas with a few game engines. Currently in love with ✨Godot✨ and kind of hating Unity >:(
    </p>
    <p>
      Check out the cards at the right side for a peek over my Steam profile, where I play almost everything, and Backlogged journal (I started with it recently, so I´ll be updating the logs from time to time). Below this you can see some personally featured projects, feel free to explore this site and find out more stuff I made ;)
    </p>
  </div>
  <div style="display: flex; flex-direction: column; align-items: flex-end;">
    <iframe
      src="https://gamer2810.github.io/steam-miniprofile/?accountId=76561198095287506&appId=367520&interactive=true&vanityId=ImJustJC"
      name="steamMiniProfilePreview" scrolling="no" frameborder="0" allowfullscreen="false"
      style="border:0px #ffffff none;" name="myiFrame" scrolling="no" frameborder="1" marginheight="0px"
      marginwidth="0px" height="300px" width="400px" allowfullscreen></iframe>
    <a href="https://backloggd.com/u/ImJustJC/" style="display: block; margin: auto;">Backloggd - ImJustJC</a>
  </div>
</div>


# Featured projects

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
