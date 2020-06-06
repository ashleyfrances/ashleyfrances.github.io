---
layout: page
permalink: /teaching/
title: teaching
description: Teaching Assistantships, guest lectures, and conference presentations.
years: [TA, Guest Lecture, Presentation]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}