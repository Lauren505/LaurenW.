---
layout: page
permalink: /publications/
title: Publications
description:
years: [2024, 2023, 2022]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}

  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

  <p>... and more to come!</p>

</div>