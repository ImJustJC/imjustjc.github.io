---
layout: single
permalink: /
lang: es
title: Inicio
page_id: landing
---

¡Hola! Soy Juan Carlos, aunque quienes me han sufrido me llaman directamente JC, y desde 2020 o por ahí me gusta intentar hacer juegos. Estudié grado y máster de Ingeniería Informática en la Universidad de Jaén y en los pocos ratos libres que tenía fuí probando a desarrollar alguna idea con motores gráficos varios. Actualmente trabajo con el Grupo de Gráficos y Geomática de la UJA desde hace un par de años ya y he publicado con ellos dos artículos científicos. Visita mi página de LinkedIn (al pie de cualquier página en todo momento, pero te lo dejo aquí tambien esta vez <a href="https://www.linkedin.com/in/juan-carlos-fernández-pérez-462622220/"><i class="fa-brands fa-linkedin"></i></a>) para más detalles sobre mi vida estudiantil y profesional, este espacio lo reservo para mis jueguicos :D

# Proyectos destacados

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