---
layout: single
title: Reseñas de juegos
lang: es
permalink: /game-reviews
page_id: game_reviews
---

{% for post in site.games limit: 5 %}
  {% include archive-single.html %}
{% endfor %}