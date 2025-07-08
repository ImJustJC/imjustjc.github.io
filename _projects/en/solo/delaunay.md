---
title: "Interactive Delaunay"
lang: en
page_id: delaunay
date: 29/06/2022
project_type: other
header_image: /assets/images/projects/delaunay_interactive/delaunayFront.png
featured: false
vertical_card: false
tags:
  - Unity
  - Windows
---

<div class="quote-shadowbox">
Interactive Delaunay triangulation generator made in Unity
</div>
<!--content-->

This project belongs to my practices from the "Geometric Algorithms" subject in the Bachelor's Degree in Computer Engineering at University of Jaén, as the final evaluation. My main target with this project was to implement the Delaunay triangulation algorithm in 2D using Unity, adding some performance optimizations to enable real time interaction. All the content made is publicly available and summarized at the following video: <a href="https://www.youtube.com/watch?v=M5Xa3ZU4OsU" target="_blank"><i class="fa-brands fa-youtube"></i></a>

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/delaunay_interactive/delaunayMassive.png" style="width: 100%; margin: auto;">
</div>

<h2>Interaction with the Delaunay</h2>

Along expected controls to add or remove points from the triangulation, I added the capability to move a point around using the cursor. Taking advantage of the algorithm efficiency and the additional improvements, the current triangulation can adapt every frame to the modified point, even against critical changes.

<div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 1.3em">
    <img style="width: 48.5%;" src="/assets/images/projects/delaunay_interactive/delaunayA.png" />
    <img style="width: 48.5%;" src="/assets/images/projects/delaunay_interactive/delaunayB.png" />
</div>

<h2>View options</h2>

<div class="flex_image_right">
  <p style="flex: 1 1 55%">Both the Delaunay triangulation and the Voronoi diagraman share a duality, from which one can be obtained from the other; this was also taken into consideration, enabling the Voronoi visualization also in real time while interacting with the points. Similarly, another property of the Delaunay holds that all circumscribed circles over each triangle don't contain any fourth point, which is also demonstrable in the project by enabling the circumscribed circle visualization.</p>
  <div style="flex: 1 1 45%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/delaunay_interactive/delaunayCircle.png">
  </div>
</div>


