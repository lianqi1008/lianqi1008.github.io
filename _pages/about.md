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

## Education

<div class="experience-list">
  <div class="experience-item">
    <img class="experience-logo" src="{{ '/assets/img/logos/sjtu.png' | relative_url }}" alt="Shanghai Jiao Tong University logo" loading="lazy" />
    <div class="experience-body">
      <div class="experience-role">Ph.D. in Information and Communication Engineering</div>
      <div class="experience-org">Shanghai Jiao Tong University · Advisors: Prof. Guo Lu and Prof. Wenjun Zhang</div>
    </div>
    <div class="experience-date">Sep 2025 – Present</div>
  </div>
  <div class="experience-item">
    <img class="experience-logo" src="{{ '/assets/img/logos/bjtu.png' | relative_url }}" alt="Beijing Jiaotong University logo" loading="lazy" />
    <div class="experience-body">
      <div class="experience-role">M.S. in Information and Communication Engineering</div>
      <div class="experience-org">Beijing Jiaotong University · Advisors: Prof. Huihui Bai and Prof. Yao Zhao</div>
    </div>
    <div class="experience-date">Sep 2022 – Jun 2025</div>
  </div>
  <div class="experience-item">
    <img class="experience-logo" src="{{ '/assets/img/logos/whut.png' | relative_url }}" alt="Wuhan University of Technology logo" loading="lazy" />
    <div class="experience-body">
      <div class="experience-role">B.S. in Software Engineering</div>
      <div class="experience-org">Wuhan University of Technology</div>
    </div>
    <div class="experience-date">Sep 2018 – Jun 2022</div>
  </div>
</div>

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

  /* --- News timeline --- */
  .news table {
    margin-bottom: 0;
  }

  .news table tr {
    position: relative;
  }

  .news table th {
    position: relative;
    width: 7.5rem !important;
    padding: 0.35rem 0.75rem 0.35rem 1.35rem;
    border: 0;
    font-size: 0.85rem;
    font-weight: 600;
    color: var(--global-theme-color);
    white-space: nowrap;
    vertical-align: top;
  }

  /* vertical line */
  .news table th::before {
    content: "";
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0.42rem;
    width: 2px;
    background: var(--global-divider-color);
  }

  .news table tr:first-child th::before {
    top: 0.75rem;
  }

  .news table tr:last-child th::before {
    bottom: auto;
    height: 0.75rem;
  }

  /* dot */
  .news table th::after {
    content: "";
    position: absolute;
    top: 0.62rem;
    left: 0.19rem;
    width: 0.52rem;
    height: 0.52rem;
    border-radius: 50%;
    background: var(--global-theme-color);
  }

  .news table td {
    padding: 0.35rem 0 0.9rem 0.5rem;
    border: 0;
    font-size: 0.93rem;
    line-height: 1.55;
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
    border-radius: 10px;
    background: var(--global-card-bg-color, var(--global-bg-color));
    transition:
      box-shadow 0.2s ease,
      border-color 0.2s ease;
  }

  .experience-item:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 35%, var(--global-divider-color));
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.06);
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
    width: 20%;
    max-width: 185px;
    margin-top: 0.3rem;
    margin-left: 2rem;
    margin-bottom: 1rem;
  }

  .post h2 {
    position: relative;
    margin-top: 2.6rem;
    margin-bottom: 1.2rem;
    padding-bottom: 0.55rem;
    font-family: Georgia, "Times New Roman", "Songti SC", STSong, SimSun, serif;
    font-size: 1.45rem;
    font-weight: 600;
    letter-spacing: 0;
    border-bottom: 1px solid var(--global-divider-color);
  }

  /* short theme-color accent on top of the divider */
  .post h2::after {
    content: "";
    position: absolute;
    bottom: -1px;
    left: 0;
    width: 2.4rem;
    height: 2px;
    background: var(--global-theme-color);
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
    padding: 1.15rem 1.3rem;
    border: 1px solid var(--global-divider-color);
    border-left: 0.28rem solid var(--global-theme-color);
    border-radius: 10px;
    background: var(--global-card-bg-color, var(--global-bg-color));
    transition:
      box-shadow 0.2s ease,
      transform 0.2s ease;
  }

  .publications ol.bibliography > li:hover,
  .publications .bibliography > li:hover {
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.07);
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
    flex: 0 0 250px;
    flex-direction: column;
    max-width: 250px;
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

  /* Venue badge and preview image share the exact same column width */
  .publications ol.bibliography > li .abbr figure,
  .publications .bibliography > li .abbr figure {
    width: 100%;
    margin: 0;
  }

  .publications ol.bibliography > li .preview,
  .publications .bibliography > li .preview {
    width: 100%;
    max-width: 100%;
    margin: auto 0 0;
  }

  .publications ol.bibliography > li .preview img,
  .publications .bibliography > li .preview img,
  .publications ol.bibliography > li img.preview,
  .publications .bibliography > li img.preview {
    display: block;
    width: 100%;
    max-width: 100%;
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    background: #fff;
    box-sizing: border-box;
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

  /* TL;DR note (second .periodical block) rendered as plain text */
  .publications ol.bibliography > li .periodical + .periodical,
  .publications .bibliography > li .periodical + .periodical {
    margin-top: 0.15rem;
    font-size: 0.84rem;
    font-style: normal;
    line-height: 1.5;
  }

  .publications ol.bibliography > li .row > div:not(.abbr),
  .publications .bibliography > li .row > div:not(.abbr) {
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
