---
layout: page
permalink: /publications/
title: publications
description: My publications in chronological order. <br> *Accepted for publication
years: [2021, 2022]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
