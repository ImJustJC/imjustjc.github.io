---
layout: single
title: My games
lang: en
permalink: /my-games
page_id: my_games
---

<div class="horizontal_card_container">
  {% assign sorted_projects = site.projects | reverse | where: 'project_type', 'game' %}
  {% for project_page in sorted_projects %}
  <div class="horizontal_card">
    <a class="title" href="{{ project_page.url | relative_url }}" rel="permalink">
      <h1>{{ project_page.title }}</h1>
    </a>
    <a class="img" href="{{ project_page.url | relative_url }}" rel="permalink">
      <img src="{{ project_page.header_image }}" style="max-width: 450px; max-height: 350px" />
    </a>
    <div class="info">
      {% assign date_day = project_page.date | date: "%d" %}
      {% assign date_month = project_page.date | date: "%m" | minus: 1 %}
      {% assign date_month_name = site.data.l10n.date_months[date_month] %}
      {% assign date_year = project_page.date | date: "%Y" %}
      <p><strong>{{ date_month_name }} - {{ date_year }}</strong> <br /> {{ project_page.excerpt | markdownify | strip_html }}</p>
    </div>
    <div class="tags">
      <h4><strong class="fas fa-fw fa-tags"></strong> Tags <strong class="fas fa-fw fa-tags"></strong></h4>
      <div class="project_grid_tag_container" style="grid-template-columns: repeat( {{ project_page.tags | size | at_most: 3 }}, max-content)">
        {% for tag_word in project_page.tags %}
          <a href="{{ tag_word | slugify | prepend: "/all-projects#" | relative_url }}" class="project_grid_tag">{{ tag_word }}</a>
        {% endfor %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>
