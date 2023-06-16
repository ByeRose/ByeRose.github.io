---
layout: page
permalink: /publications/
title: publications
description: A growing collection of your cool projects.
years: [2023, 2022, 1967, 1935]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
