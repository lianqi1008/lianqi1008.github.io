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
      <div class="experience-org">Shanghai Artificial Intelligence Laboratory · Frontier Exploration Center</div>
    </div>
    <div class="experience-date">Aug 2025 – Present</div>
  </div>
  <div class="experience-item">
    <img class="experience-logo" src="{{ '/assets/img/logos/xiaohongshu.png' | relative_url }}" alt="Xiaohongshu logo" loading="lazy" />
    <div class="experience-body">
      <div class="experience-role">Research Intern</div>
      <div class="experience-org">Xiaohongshu (RedNote) · Content Understanding Group, Applied Algorithms</div>
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
  @import url("https://cdn.jsdelivr.net/npm/@fontsource/source-serif-4@5.1.0/400.css");
  @import url("https://cdn.jsdelivr.net/npm/@fontsource/source-serif-4@5.1.0/600.css");

  /* ---------------------------------------------------------------------
   * Palette — quiet ink-teal accent. The theme's compiled main.css is not
   * shipped correctly, so the full light/dark variable sets live here.
   * ------------------------------------------------------------------- */
  :root {
    color-scheme: light;
    --global-bg-color: #ffffff;
    --global-text-color: #1a1a1a;
    --global-text-color-light: #767676;
    --global-theme-color: #0e7490;
    --global-hover-color: #0e7490;
    --global-divider-color: rgba(0, 0, 0, 0.1);
    --global-card-bg-color: #ffffff;
  }

  html[data-theme="dark"] {
    color-scheme: dark;
    --global-bg-color: #1c1c1d;
    --global-text-color: #d9d9d9;
    --global-text-color-light: #9a9aa0;
    --global-theme-color: #6cc5d4;
    --global-hover-color: #6cc5d4;
    --global-divider-color: #424246;
    --global-card-bg-color: #242428;
  }

  html,
  body {
    background: var(--global-bg-color);
    color: var(--global-text-color);
  }

  a,
  .post a,
  .post article a {
    color: var(--global-theme-color);
  }

  h1,
  h2,
  h3,
  .post-title,
  .publications .title {
    color: var(--global-text-color);
  }

  /* keep university/company logos legible on a dark background */
  html[data-theme="dark"] .experience-logo {
    background: #f4f4f5;
    padding: 3px;
    box-sizing: border-box;
  }

  html[data-theme="dark"] .profile img {
    box-shadow: 0 6px 22px rgba(0, 0, 0, 0.45);
  }

  /* soft radial tint at the top of the page */
  body::before {
    content: "";
    position: fixed;
    inset: 0 0 auto 0;
    z-index: -1;
    height: 420px;
    pointer-events: none;
    background: radial-gradient(
      900px 340px at 82% -12%,
      color-mix(in srgb, var(--global-theme-color) 8%, transparent),
      transparent 70%
    );
  }

  /* ---------------------------------------------------------------------
   * Typography
   * ------------------------------------------------------------------- */
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", Arial, sans-serif;
    font-size: 0.96rem;
    font-weight: 400;
    letter-spacing: 0.004em;
  }

  h1,
  h2,
  h3,
  .navbar-brand,
  .post-title {
    font-family: "Source Serif 4", Palatino, "Palatino Linotype", Georgia, "Songti SC", STSong, SimSun, serif;
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

  /* -----------------------------------------------------------------
   * Theme toggle — clean circular button (replaces the broken
   * half-sun-moon composite icon from the unshipped main.css)
   * ----------------------------------------------------------------- */
  .navbar .toggle-container {
    list-style: none;
  }

  #light-toggle {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2.1rem;
    height: 2.1rem;
    padding: 0;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 85%, transparent);
    border-radius: 50%;
    background: var(--global-card-bg-color, var(--global-bg-color));
    color: var(--global-text-color-light);
    font-size: 0.85rem;
    cursor: pointer;
    transition:
      color 0.2s ease,
      border-color 0.2s ease,
      background-color 0.2s ease;
  }

  #light-toggle:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 45%, transparent);
    background: color-mix(in srgb, var(--global-theme-color) 8%, transparent);
    color: var(--global-theme-color);
  }

  /* one icon at a time: moon on light, sun on dark (system = moon).
     Icons are drawn with CSS masks so they render without FontAwesome. */
  #light-toggle-system,
  #light-toggle-dark,
  #light-toggle-light {
    display: none;
    width: 1em;
    height: 1em;
    background: currentColor;
  }

  html:not([data-theme="dark"]) #light-toggle-dark {
    display: inline-block;
    -webkit-mask: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8z"/></svg>')
      center / contain no-repeat;
    mask: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8z"/></svg>')
      center / contain no-repeat;
  }

  html[data-theme="dark"] #light-toggle-light {
    display: inline-block;
    -webkit-mask: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><circle cx="12" cy="12" r="5"/><g stroke="black" stroke-width="2" stroke-linecap="round"><line x1="12" y1="1.5" x2="12" y2="4.5"/><line x1="12" y1="19.5" x2="12" y2="22.5"/><line x1="1.5" y1="12" x2="4.5" y2="12"/><line x1="19.5" y1="12" x2="22.5" y2="12"/><line x1="4.6" y1="4.6" x2="6.7" y2="6.7"/><line x1="17.3" y1="17.3" x2="19.4" y2="19.4"/><line x1="4.6" y1="19.4" x2="6.7" y2="17.3"/><line x1="17.3" y1="6.7" x2="19.4" y2="4.6"/></g></svg>')
      center / contain no-repeat;
    mask: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><circle cx="12" cy="12" r="5"/><g stroke="black" stroke-width="2" stroke-linecap="round"><line x1="12" y1="1.5" x2="12" y2="4.5"/><line x1="12" y1="19.5" x2="12" y2="22.5"/><line x1="1.5" y1="12" x2="4.5" y2="12"/><line x1="19.5" y1="12" x2="22.5" y2="12"/><line x1="4.6" y1="4.6" x2="6.7" y2="6.7"/><line x1="17.3" y1="17.3" x2="19.4" y2="19.4"/><line x1="4.6" y1="19.4" x2="6.7" y2="17.3"/><line x1="17.3" y1="6.7" x2="19.4" y2="4.6"/></g></svg>')
      center / contain no-repeat;
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
    line-height: 1.72;
  }

  /* Hide the site footer (copyright / theme credits) */
  footer {
    display: none !important;
  }

  .intro-spacer {
    height: 1.1rem;
  }

  /* ---------------------------------------------------------------------
   * Intro / header
   * ------------------------------------------------------------------- */
  .post-header .post-title {
    font-size: 2.35rem;
    font-weight: 600;
    letter-spacing: 0.01em;
  }

  .desc .intro-links {
    display: inline-flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 0.4rem;
  }

  .desc .intro-links a {
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    padding: 0.18rem 0.72rem;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 80%, transparent);
    border-radius: 999px;
    font-size: 0.83rem;
    color: var(--global-text-color);
    text-decoration: none;
    transition:
      border-color 0.2s ease,
      background-color 0.2s ease,
      color 0.2s ease;
  }

  .desc .intro-links a:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 45%, transparent);
    background: color-mix(in srgb, var(--global-theme-color) 7%, transparent);
    color: var(--global-theme-color);
  }

  .research-highlight {
    padding: 0.05rem 0.38rem;
    border-radius: 5px;
    background: color-mix(in srgb, var(--global-theme-color) 10%, transparent);
    color: var(--global-theme-color);
    font-weight: 600;
  }

  .profile {
    width: 20%;
    max-width: 185px;
    margin-top: 0.3rem;
    margin-left: 2rem;
    margin-bottom: 1rem;
  }

  .profile img {
    width: 100%;
    max-width: 100%;
    border-radius: 12px;
    box-shadow: 0 6px 22px rgba(0, 0, 0, 0.1);
  }

  /* ---------------------------------------------------------------------
   * Section headings — hairline + short gradient accent
   * ------------------------------------------------------------------- */
  .post h2 {
    position: relative;
    margin-top: 2.7rem;
    margin-bottom: 1.2rem;
    padding-bottom: 0.5rem;
    font-family: "Source Serif 4", Palatino, "Palatino Linotype", Georgia, "Songti SC", STSong, SimSun, serif;
    font-size: 1.38rem;
    font-weight: 600;
    letter-spacing: 0.01em;
    border-bottom: 1px solid color-mix(in srgb, var(--global-divider-color) 70%, transparent);
  }

  .post h2::after {
    content: "";
    position: absolute;
    bottom: -1px;
    left: 0;
    width: 2.6rem;
    height: 2px;
    border-radius: 2px;
    background: linear-gradient(90deg, var(--global-theme-color), color-mix(in srgb, var(--global-theme-color) 15%, transparent));
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

  /* ---------------------------------------------------------------------
   * News timeline
   * ------------------------------------------------------------------- */
  .news table {
    margin-bottom: 0;
  }

  .news table tr {
    position: relative;
  }

  .news table th {
    position: relative;
    width: 7rem !important;
    padding: 0.35rem 0.75rem 0.35rem 1.35rem;
    border: 0;
    font-size: 0.82rem;
    font-weight: 500;
    color: var(--global-theme-color);
    white-space: nowrap;
    vertical-align: top;
  }

  .news table th::before {
    content: "";
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0.44rem;
    width: 1.5px;
    background: color-mix(in srgb, var(--global-divider-color) 80%, transparent);
  }

  .news table tr:first-child th::before {
    top: 0.75rem;
  }

  .news table tr:last-child th::before {
    bottom: auto;
    height: 0.75rem;
  }

  .news table th::after {
    content: "";
    position: absolute;
    top: 0.64rem;
    left: 0.235rem;
    width: 0.46rem;
    height: 0.46rem;
    border-radius: 50%;
    background: var(--global-theme-color);
    box-shadow: 0 0 0 3px color-mix(in srgb, var(--global-theme-color) 14%, transparent);
  }

  .news table td {
    padding: 0.35rem 0 0.95rem 0.5rem;
    border: 0;
    font-size: 0.92rem;
    line-height: 1.6;
    color: var(--global-text-color);
  }

  .news .table,
  .news .table th,
  .news .table td {
    color: var(--global-text-color);
    background: transparent;
  }

  .news .table th {
    color: var(--global-theme-color);
  }

  /* ---------------------------------------------------------------------
   * Education & Experience cards
   * ------------------------------------------------------------------- */
  .experience-list {
    display: grid;
    gap: 0.7rem;
    margin-top: 0.75rem;
  }

  .experience-item {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 0.75rem 1.1rem;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 75%, transparent);
    border-radius: 12px;
    background: var(--global-card-bg-color, var(--global-bg-color));
    transition:
      box-shadow 0.2s ease,
      border-color 0.2s ease,
      transform 0.2s ease;
  }

  .experience-item:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 32%, var(--global-divider-color));
    box-shadow: 0 3px 14px rgba(0, 0, 0, 0.05);
    transform: translateY(-1px);
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
    font-size: 0.95rem;
    font-weight: 600;
  }

  .experience-org {
    font-size: 0.86rem;
    color: var(--global-text-color-light);
  }

  .experience-date {
    flex: 0 0 auto;
    font-size: 0.8rem;
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

  /* ---------------------------------------------------------------------
   * Publications
   * ------------------------------------------------------------------- */
  .publications .author em {
    border-bottom: 0;
    font-style: normal;
    font-weight: 700;
  }

  .publications ol.bibliography,
  .publications .bibliography {
    display: grid;
    gap: 1.05rem;
    margin-top: 0.75rem;
    padding-left: 0;
    list-style: none;
  }

  .publications ol.bibliography > li,
  .publications .bibliography > li {
    margin-bottom: 0;
    padding: 1.15rem 1.3rem;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 75%, transparent);
    border-radius: 12px;
    background: var(--global-card-bg-color, var(--global-bg-color));
    transition:
      box-shadow 0.2s ease,
      border-color 0.2s ease,
      transform 0.2s ease;
  }

  .publications ol.bibliography > li:hover,
  .publications .bibliography > li:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 32%, var(--global-divider-color));
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.06);
    transform: translateY(-2px);
  }

  .publications ol.bibliography > li .row,
  .publications .bibliography > li .row {
    display: flex;
    align-items: stretch;
    gap: 1.15rem;
    width: 100%;
    margin-right: 0;
    margin-left: 0;
  }

  .publications ol.bibliography > li .abbr,
  .publications .bibliography > li .abbr {
    display: flex;
    flex: 0 0 300px;
    flex-direction: column;
    max-width: 300px;
    padding-right: 0;
    padding-left: 0;
    text-align: center;
  }

  /* venue badge: solid venue color, white text (rule lost with main.css) */
  .publications ol.bibliography > li .abbr abbr,
  .publications .bibliography > li .abbr abbr {
    padding: 0.3rem 0;
    background-color: var(--global-theme-color);
  }

  .publications ol.bibliography > li .abbr abbr,
  .publications .bibliography > li .abbr abbr,
  .publications ol.bibliography > li .abbr abbr a,
  .publications .bibliography > li .abbr abbr a,
  .publications ol.bibliography > li .abbr abbr div,
  .publications .bibliography > li .abbr abbr div {
    color: #fff !important;
    font-size: 0.8rem;
    text-decoration: none;
  }

  .publications ol.bibliography > li .abbr abbr,
  .publications .bibliography > li .abbr abbr,
  .publications ol.bibliography > li .abbr .badge,
  .publications .bibliography > li .abbr .badge {
    display: block;
    width: 100%;
    margin-bottom: 0.7rem;
    border-radius: 7px;
    font-weight: 600;
    letter-spacing: 0.04em;
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
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 70%, transparent);
    border-radius: 8px;
    background: #fff;
    box-sizing: border-box;
  }

  .publications ol.bibliography > li .title,
  .publications .bibliography > li .title {
    margin-bottom: 0.25rem;
    font-family: "Source Serif 4", Palatino, "Palatino Linotype", Georgia, serif;
    font-size: 1.06rem;
    font-weight: 600;
    line-height: 1.4;
  }

  /* Typography hierarchy: authors > venue */
  .publications ol.bibliography > li .author,
  .publications .bibliography > li .author {
    font-size: 0.89rem;
    line-height: 1.55;
    color: var(--global-text-color);
  }

  .publications ol.bibliography > li .periodical,
  .publications .bibliography > li .periodical {
    font-size: 0.84rem;
    font-style: italic;
    color: var(--global-text-color-light);
  }

  /* TL;DR note (second .periodical block) rendered as plain text */
  .publications ol.bibliography > li .periodical + .periodical,
  .publications .bibliography > li .periodical + .periodical {
    margin-top: 0.2rem;
    font-size: 0.84rem;
    font-style: normal;
    line-height: 1.55;
    color: var(--global-text-color);
    opacity: 0.85;
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
    margin: 0.4rem 0.3rem 0 0;
    padding: 0.1rem 0.62rem;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 85%, transparent);
    border-radius: 999px;
    font-size: 0.76rem;
    letter-spacing: 0.02em;
  }

  .publications .links a.btn:hover {
    border-color: color-mix(in srgb, var(--global-theme-color) 45%, transparent);
    background: color-mix(in srgb, var(--global-theme-color) 8%, transparent);
    color: var(--global-theme-color);
  }

  /* First-author marker — tinted, lighter than a solid fill */
  .publications .links a.award {
    border-color: color-mix(in srgb, var(--global-theme-color) 35%, transparent);
    background: color-mix(in srgb, var(--global-theme-color) 10%, transparent);
    color: var(--global-theme-color) !important;
    cursor: default;
    font-weight: 600;
  }

  /* Google Scholar citation badge alignment */
  .publications .badges {
    margin-top: 0.45rem;
  }

  .publications .badges img {
    height: 1.1rem;
  }

  /* suppress the print-only duplicate of the award text */
  .publications li div.award.hidden {
    display: none !important;
  }

  .publication-note {
    margin-top: -0.35rem;
    margin-bottom: 1rem;
    font-size: 0.85rem;
    color: var(--global-text-color-light);
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
