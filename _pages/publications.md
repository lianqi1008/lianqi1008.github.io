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
  .post h1,
  .post h2 {
    font-family: Georgia, "Times New Roman", serif;
    letter-spacing: 0;
  }

  .publications .author em {
    border-bottom: 0;
    font-style: normal;
    font-weight: 700;
  }

  .publications ol.bibliography,
  .publications .bibliography {
    display: grid;
    gap: 1rem;
  }

  .publications ol.bibliography > li,
  .publications .bibliography > li {
    margin-bottom: 0;
    padding: 1.05rem 1.15rem;
    border: 1px solid var(--global-divider-color);
    border-left: 0.28rem solid var(--global-theme-color);
    border-radius: 8px;
    background: var(--global-card-bg-color, var(--global-bg-color));
  }

  .publications ol.bibliography > li .row,
  .publications .bibliography > li .row {
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    width: 100%;
    margin-right: 0;
    margin-left: 0;
  }

  .publications ol.bibliography > li .preview,
  .publications .bibliography > li .preview {
    flex: 0 0 180px;
    max-width: 180px;
    margin-right: 0;
  }

  .publications ol.bibliography > li .preview img,
  .publications .bibliography > li .preview img {
    width: 100%;
    border-radius: 6px;
  }

  .publications ol.bibliography > li .col,
  .publications .bibliography > li .col {
    flex: 1 1 0;
    max-width: none;
    padding-right: 0;
    padding-left: 0;
  }

  @media (max-width: 575.98px) {
    .publications ol.bibliography > li .row,
    .publications .bibliography > li .row {
      flex-direction: column;
    }

    .publications ol.bibliography > li .preview,
    .publications .bibliography > li .preview {
      flex-basis: auto;
      max-width: 100%;
    }
  }

  .publication-note {
    margin-top: 0.85rem;
    font-size: 0.9rem;
  }
</style>
