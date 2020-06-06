---
layout: page
permalink: /research/
title: research
description: Current research projects and upcoming publications.
years: [In Review, Manuscript in Prep, In Development]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
