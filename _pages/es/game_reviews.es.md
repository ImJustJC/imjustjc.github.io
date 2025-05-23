---
layout: single
title: Reseñas de juegos
lang: es
permalink: /reviews
page_id: reviews
---

{% for post in site.games limit: 5 %}
  {% include archive-single.html %}
{% endfor %}