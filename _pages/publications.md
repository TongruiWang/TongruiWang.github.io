---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2023, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
  
<h2>Journal Articles</h2>

{%- for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}



<h2>Preprints</h2>

{%- for y in [2023] %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}

</div>
