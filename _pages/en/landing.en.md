---
layout: single
permalink: /
lang: en
title: Home
page_id: landing
---

Hi there! I'm Juan Carlos, but everyone ends up calling me JC, and I started making games around 2020. I studied a bachelor's and master's degree at University of Jaén (UJA), taking any tiny free time I had trying to develop some game ideas with a few game engines. For now, I've been working within Graphics and Geomatics Group at UJA for a bit more than two years, and we published two research papers. Visit my LinkedIn profile (found at the footer in every page, but i'll leave it here this time <a href="https://www.linkedin.com/in/juan-carlos-fernández-pérez-462622220/"><i class="fa-brands fa-linkedin"></i></a>) for more details and references about my professional life and studies, this place is saved for my games :D

# Featured projects

<div class="vertical_card_container">
  {% assign sorted_projects = site.projects | reverse | where: 'featured', true %}
  {% for project_page in sorted_projects %}
  <div class="vertical_card">
    <a href="{{ project_page.url | relative_url }}" rel="permalink"><img src="{{ project_page.header_image }}" style="max-width: 450px; max-height: 350px" /></a>
    <a href="{{ project_page.url | relative_url }}" rel="permalink"><h1>{{ project_page.title }}</h1></a>
    {% assign date_day = project_page.date | date: "%d" %}
    {% assign date_month = project_page.date | date: "%m" | minus: 1 %}
    {% assign date_month_name = site.data.l10n.date_months[date_month] %}	
    {% assign date_year = project_page.date | date: "%Y" %}
    <p><strong>{{ date_month_name }} - {{ date_year }}</strong> <br/> {{ project_page.excerpt | markdownify | strip_html }}</p>
    <div style="width: 100%">
      <h4><strong class="fas fa-fw fa-tags"></strong> Etiquetas <strong class="fas fa-fw fa-tags"></strong></h4>
      <div class="project_grid_tag_container" style="grid-template-columns: repeat( {{ project_page.tags | size | at_most: 3 }}, max-content)">
        {% for tag_word in project_page.tags %}
          <a href="{{ tag_word | slugify | prepend: "/all-projects#" | relative_url }}" class="project_grid_tag">{{ tag_word }}</a>
        {% endfor %}
      </div>
    </div>
  </div>
  {% endfor %} 
</div>