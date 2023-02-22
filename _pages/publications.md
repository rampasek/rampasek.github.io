---
layout: page
permalink: /publications/
title: publications
description: An up-to-date list is available on <a href='https://scholar.google.com/citations?user=nqeYbJcAAAAJ'>Google Scholar</a>.
years: [2023, 2022, 2021, 2020, 2019, 2018, 2016, 2014]
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
