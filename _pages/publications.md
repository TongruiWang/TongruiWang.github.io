---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2025, 2024, 2023, 2022]
prepyears: [2025, 2024, 2023]
survyears: [2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
  
<h2>Journal Articles</h2>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}



<h2>Preprints</h2>
{%- for py in page.prepyears %}
  <h2 class="year">{{py}}</h2>
  {% bibliography -f preprints -q @*[year={{py}}]* %}
{% endfor %}



<h2>Surveys</h2>
{%- for sy in page.survyears %}
  <h2 class="year">{{sy}}</h2>
  {% bibliography -f surveys -q @*[year={{sy}}]* %}
{% endfor %}

</div>
