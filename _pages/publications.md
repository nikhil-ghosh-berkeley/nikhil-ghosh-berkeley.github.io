---
layout: page
permalink: /publications/
title: publications
description: <span>*</span> denotes equal contribution
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h3>preprints</h3>
{% bibliography -f {{site.scholar.bibliography}} --group_by none --query @*[preprint=true]* %}

<h3>conference & journal articles</h3>
{% bibliography -f {{ site.scholar.bibliography }} --query @*[preprint=false]* %}

</div>
