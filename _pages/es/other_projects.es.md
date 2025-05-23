---
layout: single
title: Otros proyectos
lang: es
permalink: /other-projects
page_id: other-projects
---

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'project_type', 'other' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
