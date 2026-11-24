---
layout: page
title: Projects
permalink: /projects/
_styles: >
  body, .navbar, h1, h2, h3, h4, .post-title { font-family: "Inter", system-ui, sans-serif; font-weight: 400; }
  .navbar .nav-link { font-size: 1rem; font-weight: 400; }
  .post-header .post-title { font-size: 2.6rem; font-weight: 700; letter-spacing: -0.02em; line-height: 1.1; color: var(--global-text-color); }
  .post-header .post-description { font-size: 1rem; line-height: 1.75; color: var(--global-text-color-light); }
  .projects h2.category { font-size: 0.8rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.14em; text-align: left; color: var(--global-theme-color); border-bottom: none; margin: 2.5rem 0 1rem; }
  .projects .card-title { font-size: 1.15rem; font-weight: 600; letter-spacing: -0.01em; color: var(--global-text-color); }
  .projects .card-text { font-size: 0.92rem; line-height: 1.6; color: var(--global-text-color-light); }
description: Selected projects.
nav: true
nav_order: 3
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
