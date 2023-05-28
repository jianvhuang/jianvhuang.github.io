---
layout: page
permalink: /publications/
title: Selected publications
description: Photos from <a href="https://unsplash.com" target="_blank">Unsplash</a>.
years: [2023, 2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
