---
layout: page
permalink: /publications/
title: Publications
description: Publications and preprints.
nav: false
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

<p class="publication-note">† Corresponding author.</p>

<style>
  .publications .author em {
    border-bottom: 0;
    font-style: normal;
    font-weight: 700;
  }

  .publication-note {
    font-size: 0.9rem;
  }
</style>
