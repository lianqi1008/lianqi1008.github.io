---
layout: about
title: About
permalink: /
subtitle: >
  [<a href="https://github.com/lianqi1008">GitHub</a>]
  [<a href="mailto:anqi.li@sjtu.edu.cn">Email</a>]
  [<a href="https://scholar.google.com/citations?user=WLFHu5cAAAAJ&hl=en">Google Scholar</a>]

profile:
  align: right
  image: profile-photo.jpg
  image_circular: false # crops the image to make it circular

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a Ph.D. student in Information and Communication Engineering at [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/), advised by Prof. Guo Lu and Prof. Wenjun Zhang. I received my M.S. degree from Beijing Jiaotong University and my B.S. degree from Wuhan University of Technology.

My research interests include vision-language models, agents, trustworthy reasoning, multimodal content moderation, and efficient visual representations.

## Publications

<div class="publications">

{% bibliography --group_by none --query @*[selected=true]* %}

</div>

<p class="publication-note">† Corresponding author.</p>

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
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", "Helvetica Neue", Arial, sans-serif;
    font-weight: 500;
  }

  .navbar {
    display: none;
  }

  .post,
  .about {
    padding-top: 0.25rem;
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
    max-width: 60%;
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

  .publication-note {
    margin-top: 0.85rem;
    margin-bottom: 2.2rem;
    font-size: 0.9rem;
  }
</style>
