---
layout: single
permalink: /
lang: en
title: Home
page_id: landing
---

Hi there! I'm Juan Carlos, but everyone ends up calling me JC, and I started making games around 2020. I studied a bachelor's and master's degree at University of Jaén (UJA), taking any tiny free time I had trying to develop some game ideas with a few game engines. For now, I've been working within Graphics and Geomatics Group at UJA for a bit more than two years, and we published two research papers. Visit my LinkedIn profile (found at the footer in every page, but i'll leave it here this time <a href="https://www.linkedin.com/in/juan-carlos-fernández-pérez-462622220/"><i class="fa-brands fa-linkedin"></i></a>) for more details and references about my professional life and studies, this place is saved for my games :D

# Featured projects

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', 'true' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
