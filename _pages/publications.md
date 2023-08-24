---
layout: page
permalink: /publications/
title: publications
description: Posted by categories in reversed chronological order.
years: [2021, 2024]
selected: true
nav: true
order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
