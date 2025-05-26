---
layout: single
lang: en
permalink: /all-projects
page_id: all_projects
---

{% assign project_tags = '' %}
{% for project_page in site.projects %}
  {% for tag in project_page.tags %}
    {% unless project_tags contains tag %}
      {% assign project_tags = project_tags | append: ';' | append: tag %}
    {% endunless %}
  {% endfor %}
{% endfor %} 

{% assign project_tags = project_tags | split: ';' | shift %}
{% for tag in project_tags %}
  <h2 id="{{ tag | slugify }}">{{ tag }}</h2>
  {% assign tagged_projects = site.projects | where_exp: 'project', 'project.tags contains tag' %}

  <div class="product-card-container">
    {% for tagged_project in tagged_projects %}
      {% include project-card.html product_page = tagged_project %}
    {% endfor %}
  </div>
{% endfor %}