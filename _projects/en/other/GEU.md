---
title: "GEU"
lang: en
page_id: geu
date: 01/01/2025
header_image: /assets/images/projects/geu/frontGEU.jpg
project_type: other
featured: true
tags:
  - Windows
  - OpenGL
  - ImGUI
---

<div class="quote-shadowbox">
Point cloud graphics engine used in research at University of Jaén.
</div>
<!--content-->

GEU (<b>G</b>eospatial and <b>E</b>nvironmental tools of <b>U</b>niversity of Jaén) is a graphics engine prototype in active development at <a href="https://gggj.ujaen.es/">Graphics and Geomatics Group of University of Jaén</a>, focused on 3D point clouds. Although it originated before, the currently used application was born around the end of 2021 as a way to unify all research labor in point clouds. Knowing the requirements and the intricacies for the methods used in research, we decided in using C++ along OpenGL, since we were learning those during my studies at that time and given their flexibility without an excessive complexity.

<img src="/assets/images/projects/geu/mainGEU.png" />

<h2>Graphical User Interface</h2>

<div style="display: flex; flex-direction: row; align-items: center; margin-bottom: 1.3em; gap: 1.5em">
  <div style="flex: 1 1 50%">
      <p>
        At the early development stages, I had the chance to build the user interface for GEU, including both GUI and inputs, which deeply interested me. To ease our workload, ImGUI was added to GEU as an external library for an easy to use graphical interface that enabled basic interaction with the engine functionality.
      </p>
      <p>
        We aimed to a familiar user interface similar to other tools like Unity or Blender, using a hierarchy of objects active in the current scene with details and distributed windows for implemented methods and functionality during research, keeping everything interactive with the mouse. Shortly after, the default ImGUI style (image at the right side) was replaced with a custom defined style that, along the defined GUI layout, is still used today (image at top).
      </p>
  </div>
  <div style="flex: 1 1 50%">
    <img src="/assets/images/projects/geu/oldGEU.png" />
  </div>
</div>

<h2>My work for GEU</h2>

Even though I focused on the user interface, my work also includes some research publications; GEU was ready quite early in development, after a year or so, for its use, and the group required some research work published ASAP.

<h3>Research papers</h3>

<ul>
  <li>
    <a href="https://diglib.eg.org/items/eab6a149-f1e2-4726-9a14-3a27e29ffd6e">An Efficient Point Selection Process over a Meshlet-structured Point Cloud</a>: In 2023 I was given a chance to publish a poster for Spanish Computer Graphics Conference 2024, showing off my research in point selection made for GEU. In short, GEU uses a point grouping-based optimization built around the graphics processor to improve rendering performance (<a href="https://developer.nvidia.com/blog/introduction-turing-mesh-shaders/"><i>meshlets</i></a>). With this structure, the point selection process can also be greatly improved without needing additional data structures. With time, this work ended up as a short publication with a talk in the congress, celebrated at Galicia.
  </li>
  <li>
    <a href="https://www.sciencedirect.com/science/article/pii/S016816992500208X">Meshlets based data model for real-time interaction and analysis with hyper-spectral vegetation data</a>: With a first paper published, a second one came shortly after, targeting a journal this time. While staying on the same basics, we tried to exploit the optimization structure used by GEU, achieving a promising method to improve storage usage and analysis quality with a huge set of data over point clouds. All was implemented in GEU, proving the application scalability and enabling this method to be used for the other researchers.
  </li>
</ul>

