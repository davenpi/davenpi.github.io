---
layout: page
title: hobbies
permalink: /hobbies/
description: Some things I like to do.
nav: true
nav_order: 2
display_categories:
horizontal: false
---

<!-- pages/hobbies.md -->
<div class="hobbies">
{%- if site.enable_hobby_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include hobbies.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_hobbies = site.hobbies | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
      <h2> HI. I am inside the hobbies md file</h2>
    {%- for project in sorted_hobbies -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for hobby in sorted_hobbies -%}
      {% include hobbies.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
