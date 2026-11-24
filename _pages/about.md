---
layout: default
title: About
permalink: /
---

<style>
  body, .navbar, h1, h2, h3, h4 { font-family: "Inter", system-ui, sans-serif; font-weight: 400; }
  .navbar .nav-link { font-size: 1rem; font-weight: 400; }
  .home { max-width: 880px; margin: 0 auto; padding-top: 1.5rem; }
  .home a { text-decoration: none; }
  .home-hero { display: grid; grid-template-columns: 1fr 200px; gap: 3rem; align-items: center; }
  .home-name { font-size: 2.6rem; font-weight: 700; letter-spacing: -0.02em; line-height: 1.1; margin: 0 0 1.25rem; color: var(--global-text-color); }
  .home-name-zh { font-size: 1.5rem; font-weight: 500; letter-spacing: 0.05em; margin-left: 0.4rem; color: var(--global-text-color-light); }
  .home-bio { font-size: 1rem; line-height: 1.75; color: var(--global-text-color); }
  .home-bio strong { font-weight: 700; }
  .home-photo img { width: 200px; height: 250px; object-fit: cover; border-radius: 50% / 42%; border: 4px solid var(--global-bg-color); box-shadow: 0 0 0 2px var(--global-theme-color); }
  .home-photo { text-align: center; }
  .home-location { margin-top: 0.75rem; font-family: "JetBrains Mono", ui-monospace, Consolas, monospace; font-size: 0.85rem; color: var(--global-text-color-light); }
  .home-links { display: flex; flex-wrap: wrap; gap: 0.6rem; margin-top: 1.5rem; }
  .home-links a { display: inline-flex; align-items: center; gap: 0.45rem; padding: 0.4rem 0.95rem; border: 1.5px solid var(--global-text-color); border-radius: 999px; font-size: 1rem; font-weight: 400; color: var(--global-text-color); transition: all 0.15s ease; }
  .home-links a:hover { border-color: var(--global-theme-color); color: var(--global-theme-color); }
  .home-section { margin-top: 3.5rem; }
  .home-section h2 { font-size: 0.8rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.14em; color: var(--global-theme-color); margin-bottom: 1.25rem; }
  .home-timeline { list-style: none; padding: 0; margin: 0; border-left: 2px solid var(--global-divider-color); }
  .home-timeline li { position: relative; padding: 0 0 1.4rem 1.4rem; }
  .home-timeline li:last-child { padding-bottom: 0; }
  .home-timeline li::before { content: ""; position: absolute; left: -7px; top: 0.4rem; width: 12px; height: 12px; border-radius: 50%; background: var(--global-bg-color); border: 2px solid var(--global-theme-color); }
  .home-timeline .org { font-weight: 600; color: var(--global-text-color); }
  .home-timeline .detail { font-size: 0.92rem; color: var(--global-text-color-light); }
  @media (max-width: 700px) {
    .home-hero { grid-template-columns: 1fr; gap: 1.5rem; }
    .home-photo { order: -1; }
    .home-photo img { width: 150px; height: 188px; }
    .home-name { font-size: 2.1rem; }
  }
</style>

<div class="home">
  <section class="home-hero">
    <div>
      <h1 class="home-name">Fan-Yi Hsu <span class="home-name-zh" lang="zh-Hant">徐凡懿</span></h1>
      <p class="home-bio">
        Hello, I am a <strong>Computer Science</strong> undergraduate at <strong>National Yang Ming Chiao Tung University (NYCU)</strong>, Taiwan.
        I am currently conducting research with
        <a href="https://homepage.citi.sinica.edu.tw/pages/yu.tsao/index_en.html" target="_blank" rel="noopener">Prof. Yu Tsao</a> at
        <strong>Academia Sinica</strong> and <a href="https://aseschng.github.io/default.html" target="_blank" rel="noopener">Prof. Eng Siong Chng</a> at
        <strong>Nanyang Technological University (NTU)</strong>, Singapore. I am interested in developing
        <strong>robust and efficient learning methods</strong> that generalize across diverse real-world conditions.
      </p>
      <div class="home-links">
        <a href="mailto:fanyi194.cs12@nycu.edu.tw"><i class="fa-solid fa-envelope"></i> Email</a>
        <a href="https://github.com/FLYIH" target="_blank" rel="noopener"><i class="fa-brands fa-github"></i> GitHub</a>
        <a href="https://scholar.google.com/citations?hl=en&user=zKL2VA8AAAAJ" target="_blank" rel="noopener"><i class="ai ai-google-scholar"></i> Scholar</a>
        <a href="https://www.linkedin.com/in/fan-yi-hsu-a123452b4/" target="_blank" rel="noopener"><i class="fa-brands fa-linkedin"></i> LinkedIn</a>
      </div>
    </div>
    <div class="home-photo">
      <img src="{{ 'assets/img/prof_pic.jpg' | relative_url }}" alt="Fan-Yi Hsu">
      <div class="home-location">Hsinchu, Taiwan</div>
    </div>
  </section>
  <section class="home-section">
    <h2>Education</h2>
    <ul class="home-timeline">
      <li>
        <div class="org">National Yang Ming Chiao Tung University</div>
        <div class="detail">B.S. in Computer Science</div>
      </li>
      <li>
        <div class="org">National Experimental High School at Hsinchu Science Park</div>
      </li>
    </ul>
  </section>
</div>
