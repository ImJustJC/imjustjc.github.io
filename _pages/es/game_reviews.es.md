---
layout: single
title: Reseñas de juegos
lang: es
permalink: /reviews
page_id: reviews
---

{% for post in site.games reversed %}
  {% include archive-single.html %}
{% endfor %}