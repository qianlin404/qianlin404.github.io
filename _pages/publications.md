---
layout: page
permalink: /publications/
title: publications
description: publications by years in reversed chronological order.
years: [2024, 2023, 2020, 2017, 2016] 
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
