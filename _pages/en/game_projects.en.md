---
layout: single
title: My games
lang: en
permalink: /games
page_id: games
---

<div class="product-card-container">
  {% assign sorted_projects = site.projects | reverse | where: 'project_type', 'game' %}
  {% for project_page in sorted_projects %}
    {% include project-card.html product_page = project_page %}
  {% endfor %}
</div>
