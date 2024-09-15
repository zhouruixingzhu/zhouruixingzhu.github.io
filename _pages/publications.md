---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order. 
years: [2024,2023]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<i>See <a href="https://scholar.google.com.hk/citations?user=bKNg57IAAAAJ&hl=zh-CN&oi=ao">Google Scholar</a> for my up-to-date publications.</i>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
