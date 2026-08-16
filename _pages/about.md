---
layout: about
title: About
permalink: /
subtitle: >
  <span class="intro-links">
  <a href="https://github.com/lianqi1008"><i class="fa-brands fa-github"></i> GitHub</a>
  <a href="https://scholar.google.com/citations?user=WLFHu5cAAAAJ&hl=en"><i class="fa-solid fa-graduation-cap"></i> Google Scholar</a>
  <a href="mailto:anqi.li@sjtu.edu.cn"><i class="fa-solid fa-envelope"></i> Email</a>
  </span>

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

I am a Ph.D. student in Information and Communication Engineering at [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/), advised by **<u>Prof. Guo Lu</u>** and **<u>Prof. Wenjun Zhang</u>**. I received my M.S. degree from Beijing Jiaotong University and my B.S. degree from Wuhan University of Technology.

My research focuses on <span class="research-highlight">LLM post-training</span> and <span class="research-highlight">AIGC</span> — aligning and enhancing large models after pre-training, and building generative models for visual and multimodal content.

<div class="intro-spacer"></div>

## News

{% include news.liquid %}

## Experience

<div class="experience-list">
  <div class="experience-item">
    <img class="experience-logo" src="{{ '/assets/img/logos/shanghai-ai-lab.png' | relative_url }}" alt="Shanghai AI Laboratory logo" loading="lazy" />
    <div class="experience-body">
      <div class="experience-role">Research Intern</div>
      <div class="experience-org">Shanghai Artificial Intelligence Laboratory</div>
    </div>
    <div class="experience-date">Aug 2025 – Present</div>
  </div>
  <div class="experience-item">
    <img class="experience-logo" src="{{ '/assets/img/logos/xiaohongshu.png' | relative_url }}" alt="Xiaohongshu logo" loading="lazy" />
    <div class="experience-body">
      <div class="experience-role">Research Intern</div>
      <div class="experience-org">Xiaohongshu (RedNote)</div>
    </div>
    <div class="experience-date">Jul 2024 – Jul 2025</div>
  </div>
</div>

## Publications

<p class="publication-note">† Corresponding author.</p>

<div class="publications">

{% bibliography --group_by none --query @*[selected=true]* %}

</div>

## Services

- Reviewer, ECCV 2026

<style>
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", Arial, sans-serif;
    font-weight: 400;
  }

  h1,
  h2,
  h3,
  .navbar-brand,
  .post-title {
    font-family: Georgia, "Times New Roman", "Songti SC", STSong, SimSun, serif;
    font-weight: 600;
  }

  /* Hide navbar chrome but keep the dark-mode toggle accessible */
  .navbar {
    padding: 0.25rem 0.75rem;
    background: transparent !important;
    border-bottom: none;
    box-shadow: none !important;
  }

  .navbar .navbar-brand,
  .navbar .navbar-toggler,
  .navbar .navbar-menu-list > li:not(.toggle-container) {
    display: none !important;
  }

  .navbar .navbar-collapse {
    display: flex !important;
    flex-basis: auto;
    justify-content: flex-end;
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

  .post article > .clearfix > p {
    max-width: 96%;
    margin-bottom: 1.05rem;
  }

  /* Hide the site footer (copyright / theme credits) */
  footer {
    display: none !important;
  }

  .intro-spacer {
    height: 1.1rem;
  }

  /* --- Intro / header area --- */
  .post-header .post-title {
    font-family: Georgia, "Times New Roman", serif;
    font-weight: 600;
    letter-spacing: 0.01em;
  }

  .desc .intro-links {
    display: inline-flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.35rem;
  }

  .desc .intro-links a {
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    padding: 0.22rem 0.75rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.85rem;
    color: var(--global-text-color);
    text-decoration: none;
    transition:
      border-color 0.2s ease,
      color 0.2s ease;
  }

  .desc .intro-links a:hover {
    border-color: var(--global-theme-color);
    color: var(--global-theme-color);
  }

  .research-highlight {
    padding: 0.05rem 0.35rem;
    border-radius: 4px;
    background: color-mix(in srgb, var(--global-theme-color) 12%, transparent);
    color: var(--global-theme-color);
    font-weight: 600;
  }

  .profile-location {
    margin-top: 0.4rem;
    font-size: 0.82rem;
    color: var(--global-text-color-light);
    text-align: center;
  }

  /* --- Experience --- */
  .experience-list {
    display: grid;
    gap: 0.75rem;
    margin-top: 0.75rem;
  }

  .experience-item {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 0.8rem 1.15rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    background: var(--global-card-bg-color, var(--global-bg-color));
  }

  .experience-logo {
    flex: 0 0 44px;
    width: 44px;
    height: 44px;
    border-radius: 8px;
    object-fit: contain;
  }

  .experience-body {
    flex: 1 1 auto;
    min-width: 0;
  }

  .experience-role {
    font-size: 0.98rem;
    font-weight: 600;
  }

  .experience-org {
    font-size: 0.88rem;
    color: var(--global-text-color-light);
  }

  .experience-date {
    flex: 0 0 auto;
    font-size: 0.82rem;
    color: var(--global-text-color-light);
    white-space: nowrap;
  }

  @media (max-width: 575.98px) {
    .experience-item {
      flex-wrap: wrap;
    }

    .experience-date {
      flex-basis: 100%;
      margin-left: calc(44px + 1rem);
    }
  }

  .profile {
    width: 24%;
    max-width: 220px;
    margin-top: 0.3rem;
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
    width: 100%;
    max-width: 100%;
    border-radius: 10px;
    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.12);
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
    transition:
      box-shadow 0.2s ease,
      transform 0.2s ease;
  }

  .publications ol.bibliography > li:hover,
  .publications .bibliography > li:hover {
    box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
    transform: translateY(-2px);
  }

  .publications ol.bibliography > li .row,
  .publications .bibliography > li .row {
    display: flex;
    align-items: stretch;
    gap: 1rem;
    width: 100%;
    margin-right: 0;
    margin-left: 0;
  }

  .publications ol.bibliography > li .abbr,
  .publications .bibliography > li .abbr {
    display: flex;
    flex: 0 0 210px;
    flex-direction: column;
    max-width: 210px;
    padding-right: 0;
    padding-left: 0;
    text-align: center;
  }

  .publications ol.bibliography > li .abbr abbr,
  .publications .bibliography > li .abbr abbr,
  .publications ol.bibliography > li .abbr .badge,
  .publications .bibliography > li .abbr .badge {
    display: block;
    width: 100%;
    margin-bottom: 0.75rem;
  }

  .publications ol.bibliography > li .preview,
  .publications .bibliography > li .preview {
    width: 100%;
    max-width: 210px;
    margin: auto 0 0;
  }

  .publications ol.bibliography > li .preview img,
  .publications .bibliography > li .preview img {
    width: 100%;
    border-radius: 6px;
  }

  .publications ol.bibliography > li .title,
  .publications .bibliography > li .title {
    margin-bottom: 0.2rem;
    font-family: Georgia, "Times New Roman", serif;
    font-size: 1.08rem;
    font-weight: 600;
    line-height: 1.35;
  }

  /* Typography hierarchy: authors > venue */
  .publications ol.bibliography > li .author,
  .publications .bibliography > li .author {
    font-size: 0.9rem;
    line-height: 1.5;
    color: var(--global-text-color);
  }

  .publications ol.bibliography > li .periodical,
  .publications .bibliography > li .periodical {
    font-size: 0.85rem;
    font-style: italic;
    color: var(--global-text-color-light);
  }

  .publications ol.bibliography > li .col,
  .publications .bibliography > li .col {
    flex: 1 1 0;
    max-width: none;
    padding-right: 0;
    padding-left: 0;
  }

  .publications ol.bibliography > li .abbr + .col,
  .publications .bibliography > li .abbr + .col {
    padding-left: 0;
  }

  /* Link buttons (arXiv / Code / ...) rendered as subtle pills */
  .publications .links a.btn,
  .publications .links a.award {
    margin: 0.35rem 0.3rem 0 0;
    padding: 0.12rem 0.6rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.78rem;
    letter-spacing: 0.02em;
  }

  .publications .links a.btn:hover {
    border-color: var(--global-theme-color);
    color: var(--global-theme-color);
  }

  /* First-author marker */
  .publications .links a.award {
    border-color: var(--global-theme-color);
    background: var(--global-theme-color);
    color: var(--global-bg-color);
    cursor: default;
    font-weight: 600;
  }

  /* Google Scholar citation badge alignment */
  .publications .badges {
    margin-top: 0.45rem;
  }

  .publications .badges img {
    height: 1.15rem;
  }

  .publication-note {
    margin-top: -0.35rem;
    margin-bottom: 1rem;
    font-size: 0.9rem;
  }

  @media (max-width: 575.98px) {
    .profile {
      width: 36%;
      max-width: 170px;
      margin-left: 1rem;
    }

    .publications ol.bibliography > li .row,
    .publications .bibliography > li .row {
      flex-direction: column;
    }

    .publications ol.bibliography > li .abbr,
    .publications .bibliography > li .abbr,
    .publications ol.bibliography > li .preview,
    .publications .bibliography > li .preview {
      flex-basis: auto;
      max-width: 100%;
    }
  }
</style>
