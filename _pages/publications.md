---
layout: page
permalink: /publications/
title: Publications
description: A list of my publications during my undergraduate and postgraduate years.       ... More to come ... 
years: [2023, 2021, 2020]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
