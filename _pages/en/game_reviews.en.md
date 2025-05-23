---
layout: single
title: Game reviews
lang: en
permalink: /reviews
page_id: reviews
---

{% for post in site.games limit: 5 %}
  {% include archive-single.html %}
{% endfor %}