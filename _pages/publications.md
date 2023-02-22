---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: []
nav: true
nav_order: 1
sort_by: year
order: descending
---
<!-- _pages/publications.md -->
<div class="publications">

  <h2 class="preprint">Preprint(s) </h2>
  {% bibliography -f papers -q @preprint %}

  <h2 class="article">International journal papers </h2>
  {% bibliography -f papers -q @article %}

  <h2 class="international_conf">International conference papers </h2>
  {% bibliography -f papers -q @inproceedings[language!=French] %}

  <h2 class="national_conf">National conference papers </h2>
  {% bibliography -f papers -q @inproceedings[language=French] %}

  <h2 class="tech_report">Technical reports </h2>
  {% bibliography -f papers -q @techreport %}

  <h2 class="thesis">Thesis </h2>
  {% bibliography -f papers -q @phdthesis %}

</div>