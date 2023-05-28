---
layout: page
permalink: /publications/
title: Publications
description: An up-to-date list is available on <a href="https://scholar.google.com/citations?user=atD6GcMAAAAJ&hl=en" target="_blank">Google Scholar</a>.
years: [2023, 2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
