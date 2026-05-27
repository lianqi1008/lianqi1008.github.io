---
layout: about
title: About
permalink: /
subtitle: >
  [<a href="https://github.com/lianqi1008">GitHub</a>]
  [<a href="https://scholar.google.com/citations?user=WLFHu5cAAAAJ&hl=en">Google Scholar</a>]
  [<a href="mailto:anqi.li@sjtu.edu.cn">Email</a>]

profile:
  align: right
  image: profile-photo.jpg
  image_circular: false # crops the image to make it circular

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a Ph.D. student in Information and Communication Engineering at [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/), advised by **<u>Prof. Guo Lu</u>** and **<u>Prof. Wenjun Zhang</u>**. I received my M.S. degree from Beijing Jiaotong University and my B.S. degree from Wuhan University of Technology.

My research interests include vision-language models, agents, trustworthy reasoning, multimodal content moderation, and efficient visual representations.

## Publications

<p class="publication-note">† Corresponding author.</p>

<div class="publications">

{% bibliography --group_by none --query @*[selected=true]* %}

</div>

## Services

- Reviewer, ECCV 2026

<style>
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", "Helvetica Neue", Arial, sans-serif;
    font-weight: 400;
  }

  h1,
  h2,
  h3,
  .navbar-brand,
  .post-title {
    font-family: Georgia, "Times New Roman", serif;
    font-weight: 600;
  }

  .navbar {
    display: none;
  }

  .post,
  .about {
    padding-top: 0.25rem;
  }

  .post article {
    max-width: 100%;
  }

  .post article > .clearfix {
    width: 100%;
  }

  .profile {
    width: 36%;
    max-width: 320px;
    margin-left: 2rem;
    margin-bottom: 1rem;
  }

  .post h2 {
    margin-top: 2.6rem;
    margin-bottom: 1.1rem;
    font-family: Georgia, "Times New Roman", serif;
    font-size: 1.45rem;
    font-weight: 600;
    letter-spacing: 0;
  }

  .post h2:first-of-type {
    margin-top: 2.2rem;
  }

  .social {
    font-size: 0.86rem;
  }

  .social a,
  .social i,
  .social svg {
    font-size: 0.92em;
  }

  .profile img {
    width: 72%;
    max-width: 72%;
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
    margin-top: 0.75rem;
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

  .publication-note {
    margin-top: -0.35rem;
    margin-bottom: 1rem;
    font-size: 0.9rem;
  }

  @media (max-width: 575.98px) {
    .profile {
      width: 45%;
      max-width: 240px;
      margin-left: 1rem;
    }

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
</style>
