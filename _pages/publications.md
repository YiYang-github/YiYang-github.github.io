---
layout: page
permalink: /publications/
title: publications
description: "(&#x2A) denotes equal contribution"
years: [2025, 2024, 2023]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

