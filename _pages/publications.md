---
layout: page
permalink: /publications/
title: publications
description: Publications.
years: [2014,2016,2020]
nav: true
---

<div class="publications">

<h1 class="post-title"> Published </h1>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1 class="post-title"> Working papers / Under review </h1>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f working -q @*[year={{y}}]* %}
{% endfor %}

<h1 class="post-title"> Conferences and Talks </h1>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>
