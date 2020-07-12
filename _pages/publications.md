---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order.
years: [1956, 1950, 1935, 1905]
nav: true
---

<h2>Conferences</h2>
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


<h2>Preprints</h2>
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f preprint -q @*[year={{y}}]* %}
{% endfor %}

</div>
