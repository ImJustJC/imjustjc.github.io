---
title: "GEU"
lang: en
page_id: geu
date: 30/06/2025
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

GEU (<b>G</b>eospatial and <b>E</b>nvironmental tools of <b>U</b>niversity of Jaén) is a graphics engine prototype in active development at <a href="https://gggj.ujaen.es/">Graphics and Geomatics Group of University of Jaén</a>, focused on 3D point clouds. Although it originated before, the currently used application was born around the end of 2021 as a way to unify all research labor in point clouds. Knowing the requirements and the intricacies for the methods used in research, we decided in using C++ along OpenGL, since we were learning those during our studies at that time and given their flexibility without an excessive complexity.

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/geu/mainGEU.png" style="width: 100%; margin: auto;">
</div>

<h2>Graphical User Interface</h2>

<div style="align-items: center; margin-bottom: 1.3em; gap: 1.5em">
  <p>
    At the early development stages, I had the chance to build the user interface for GEU, including both GUI and inputs, which deeply interested me. To ease our workload, ImGUI was added to GEU as an external library for an easy to use graphical interface that enabled basic interaction with the engine functionality.
  </p>
  <p>
    We aimed to a familiar user interface similar to other tools like Unity or Blender, using a hierarchy of objects active in the current scene with details and distributed windows for implemented methods and functionality during research, keeping everything interactive with the mouse. Shortly after, the default ImGUI style was replaced with a custom defined style that, along the defined GUI layout, is still used today.
  </p>
</div>

<div style="display: grid; grid-template-columns: repeat(2, 1fr); justify-items: center; column-gap: 1.3rem;">
  <p><strong>Screen capture from the latest GEU version</strong></p>
  <p><strong>Screen capture from the original GEU version</strong></p>
  <img src="/assets/images/projects/geu/hyperGEU.png" alt="Screen capture from the latest GEU version">
  <img src="/assets/images/projects/geu/oldGEU.png" alt="Screen capture from the original GEU version">
</div>

<h2>Functionality modules</h2>

<div class="flex_image_right">
  <div style="flex: 1 1 55%">
      <p>
        Apart from rendering purposes, GEU required a precise management for spectral imaging data and analysis, where the main effort is made within the research group. Since all additional utilities are not really paired with the graphical engine shenanigans and developed by other members, a module system was designed, allowing every single module focus on a specific functionality and abstracting it from the rest of the application.
      </p>
      <p>
        At first, these modules where added directly on the project, but it wouldn't scale properly against more and more developers joining the group. This made me start working on a reimplementation for the entire module system, using a dynamic approach instead: this way, a module is added in runtime by the user instead of loading all of them at the start. The new system is implemented via Dynamic Link Libraries (DLL) on Windows, and proved to be a useful addition for both the users and other developers.
      </p>
  </div>
  <div style="flex: 1 1 45%; align-items: end; text-align: right;">
    <img src="/assets/images/projects/geu/modulesGEU.png" />
  </div>
</div>

<h2>Spectral imaging and data fusion</h2>

Building a rendering engine, although useful, was not enough for the research group. As mentioned, many specific utilities were needed, and so was implemented the module system. Since then, many more modules were added, but data fusion was crucial and the first category implemented. Data fusion means fusing spectral imaging with spatial data from point clouds; this is, taking a scanned point cloud and spectral dataset, and extending every point in the cloud with its respective spectral data.

Our work spanned three types of spectral sensors: thermal, multispectral, and <strong>hyperspectral</strong>. For me, I ended up charged with hyperspectral fusion, a real challenge due to the massive datasets used, requiring many tweaks to ensure a proper performance. At the same time, this fusion made the entry point for a hyperspectral analysis module and opportunities for research papers arose. The next image shows a quick look for hyperspectral signature over a selected area, using the real data (orange graph) compared to our implemented system (blue graph), using aggregated data with a much more performant process:

<div style="margin-bottom: 1.3em; display: flex; flex-direction: column;">
  <img src="/assets/images/projects/geu/hyperDataGEU.png" style="width: 100%; margin: auto;">
</div>

<h2>My research using GEU</h2>

Along all work I made for the GEU engine overall, I also published some research during those years:

<h3>Research papers</h3>

<ul>
  <li>
    <a href="https://diglib.eg.org/items/eab6a149-f1e2-4726-9a14-3a27e29ffd6e">An Efficient Point Selection Process over a Meshlet-structured Point Cloud</a>: In 2023 I was given a chance to publish a poster for Spanish Computer Graphics Conference 2024, showing off my research in point selection made for GEU. In short, GEU uses a point grouping-based optimization built around the graphics processor to improve rendering performance (<a href="https://developer.nvidia.com/blog/introduction-turing-mesh-shaders/"><i>meshlets</i></a>). With this structure, the point selection process can also be greatly improved without needing additional data structures. With time, this work ended up as a short publication with a talk in the congress, celebrated at Galicia.
  </li>
  <li>
    <a href="https://www.sciencedirect.com/science/article/pii/S016816992500208X">Meshlets based data model for real-time interaction and analysis with hyper-spectral vegetation data</a>: With a first paper published, a second one came shortly after, targeting a journal this time. While staying on the same basics, we tried to exploit the optimization structure used by GEU, achieving a promising method to improve storage usage and analysis quality with a huge set of data over point clouds. All was implemented in GEU, proving the application scalability and enabling this method to be used for the other researchers.
  </li>
</ul>

