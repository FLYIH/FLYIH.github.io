---
layout: page
title: Course Review Platform
description: A course and advisor review platform for NYCU students.
img: assets/img/projects/course-review.png
importance: 1
---

<style>
  html:not([data-theme="dark"]) {
    --global-bg-color: #e0d9ce; --global-card-bg-color: #eae6e0; --global-text-color: #3b2f1e; --global-text-color-light: #7a6a55;
    --global-theme-color: #1f8a4c; --global-hover-color: #1f8a4c; --global-divider-color: rgba(59, 47, 30, 0.15);
    --global-footer-bg-color: #3b2f1e; --global-footer-text-color: #e0d9ce; --global-footer-link-color: #ffffff;
  }
  .cr { --cr-bg: #d4cabb; --cr-card: #eae6e0; --cr-ink: #3b2f1e; --cr-green: #1f8a4c; --cr-yellow: #f5b800; }
  .cr-frame.cr-video { background: none; padding: 0; }
  .cr-link { display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.5rem 1.1rem; border: 1.5px solid var(--global-text-color); border-radius: 999px; color: var(--global-text-color); font-size: 1rem; text-decoration: none; }
  .cr-link:hover { border-color: var(--global-theme-color); color: var(--global-theme-color); text-decoration: none; }
  .cr-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; margin: 1rem 0 2rem; }
  .cr-tag { padding: 0.15rem 0.7rem; border-radius: 999px; font-size: 0.85rem; font-weight: 600; }
  .cr-tag.green { background: var(--cr-green); color: #fff; }
  .cr-tag.yellow { background: var(--cr-yellow); color: var(--cr-ink); }
  .cr-frame { background: var(--cr-bg); border-radius: 14px; padding: 1.25rem; margin-bottom: 2.5rem; }
  .cr-frame img, .cr-frame video, .cr-frame iframe { display: block; width: 100%; border-radius: 8px; box-shadow: 0 2px 10px rgba(59, 47, 30, 0.18); }
  .cr-frame iframe { aspect-ratio: 16 / 9; height: auto; border: 0; }
  .cr h2 { font-size: 0.8rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.14em; color: var(--global-theme-color); margin: 2.5rem 0 1rem; }
  .cr-features { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1rem; }
  .cr, .cr p, .cr li { font-size: 1rem; line-height: 1.7; }
  .cr-feature { background: transparent; color: var(--cr-ink); border: 1.5px solid var(--global-text-color); border-radius: 12px; padding: 1rem 1.2rem; }
  .cr-feature h3 { font-size: 1rem; font-weight: 600; margin: 0 0 0.3rem; color: var(--cr-ink); }
  .cr-feature p { margin: 0; }
  .cr-features.filled .cr-feature { background: var(--cr-card); border: none; }
  .cr-meta { display: flex; flex-wrap: wrap; gap: 2.5rem; margin: 0.5rem 0 2rem; }
  .cr-meta > div { display: flex; flex-direction: column; gap: 0.15rem; }
  .cr-meta .k { font-size: 0.75rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; color: var(--global-text-color-light); }
  .cr-meta .v { font-size: 1rem; font-weight: 600; color: var(--global-text-color); }
  .cr-feature h3 i { margin-right: 0.35rem; color: var(--cr-green); }
  .cr-stat { display: flex; align-items: center; gap: 1.25rem; margin: 1.5rem 0 2rem; padding: 1.1rem 1.4rem; background: var(--cr-card); border-radius: 12px; }
  .cr-stat .num { font-size: 2.4rem; font-weight: 700; letter-spacing: -0.02em; color: var(--cr-green); line-height: 1; }
  .cr-stat .label { font-size: 1rem; line-height: 1.7; color: var(--cr-ink); }
  .cr-stack { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; }
  .cr-stack > div { display: flex; flex-direction: column; align-items: flex-start; gap: 0.4rem; background: var(--cr-card); border-radius: 12px; padding: 0.9rem 1.1rem; }
  .cr-stack .k { font-size: 0.78rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; color: var(--global-text-color-light); }
  @media (max-width: 700px) { .cr-features { grid-template-columns: 1fr; } .cr-stack { grid-template-columns: repeat(2, 1fr); } .cr-stat { flex-direction: column; align-items: flex-start; gap: 0.5rem; } }
</style>

<div class="cr">
  <a class="cr-link" href="https://nctuplus.top/comment" target="_blank" rel="noopener"><i class="fa-solid fa-arrow-up-right-from-square"></i> nctuplus.top</a>
  <div class="cr-tags">
    <span class="cr-tag green">Web App</span>
    <span class="cr-tag yellow">NYCU</span>
  </div>
  <div class="cr-frame cr-video">
    <iframe src="https://www.youtube-nocookie.com/embed/-sc9pzBszFA?rel=0" title="Course Review Platform demo" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy"></iframe>
  </div>
  <div class="cr-meta">
    <div><span class="k">Timeline</span><span class="v">2024.07 – Present</span></div>
    <div><span class="k">Team</span><span class="v">4 members</span></div>
    <div><span class="k">Role</span><span class="v">Engineer → Team Lead</span></div>
  </div>
  <h2>Overview</h2>
  <p>
    <strong>NCTU+</strong> is a course and advisor review platform for NYCU students. Users publish structured reviews covering course content,
    workload, grading, and final grade, then search them by course, instructor, or tag before enrolling.
    The system is a React.js frontend backed by a Go API and MySQL, deployed with Docker.
  </p>
  <div class="cr-stat">
    <span class="num">100+</span>
    <span class="label">students have published reviews on the platform.</span>
  </div>
  <h2>Features</h2>
  <div class="cr-features">
    <div class="cr-feature">
      <h3>Course reviews</h3>
      <p>Structured reviews with department, instructor, workload and grading ratings, and final grade.</p>
    </div>
    <div class="cr-feature">
      <h3>Advisor reviews</h3>
      <p>A separate section for experiences with thesis and project advisors.</p>
    </div>
    <div class="cr-feature">
      <h3>Keyword search</h3>
      <p>Search across all reviews by course name, instructor, or keyword.</p>
    </div>
    <div class="cr-feature">
      <h3>Anonymous posting</h3>
      <p>Students can post reviews anonymously and browse them with instructor and course tags.</p>
    </div>
  </div>
  <h2>My Role</h2>
  <div class="cr-features filled">
    <div class="cr-feature">
      <h3><i class="fa-brands fa-react"></i> Review Posting Page</h3>
      <p>Built the page where students write and publish reviews in React.js.</p>
    </div>
    <div class="cr-feature">
      <h3><i class="fa-solid fa-spider"></i> Course Data Crawler</h3>
      <p>Wrote a crawler that collects course information, so students pick a course from a list instead of typing it when posting.</p>
    </div>
    <div class="cr-feature">
      <h3><i class="fa-solid fa-magnifying-glass"></i> Course Display &amp; Tag Search</h3>
      <p>Redesigned how courses are displayed and added search by instructor and course tags.</p>
    </div>
    <div class="cr-feature">
      <h3><i class="fa-solid fa-server"></i> Server Operations</h3>
      <p>Sole maintainer of the production server: resolved outages and managed database backups for the Dockerized deployment.</p>
    </div>
    <div class="cr-feature" style="grid-column: 1 / -1">
      <h3><i class="fa-solid fa-people-group"></i> Team Lead</h3>
      <p>Started as an engineer and later took over leading the four-person team.</p>
    </div>
  </div>
  <h2>Tech Stack</h2>
  <div class="cr-stack">
    <div><span class="k">Frontend</span><span class="cr-tag green">React.js</span></div>
    <div><span class="k">Backend</span><span class="cr-tag yellow">Go</span></div>
    <div><span class="k">Database</span><span class="cr-tag yellow">MySQL</span></div>
    <div><span class="k">Deployment</span><span class="cr-tag green">Docker</span></div>
  </div>
</div>
