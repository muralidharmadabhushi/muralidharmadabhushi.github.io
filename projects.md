---
layout: default
title: Projects
nav_id: projects
permalink: /projects.html
---

### Projects

My projects are organized as broad research categories. Each category page contains smaller sub-projects with short descriptions, figures, and related paper links.

<div class="project-grid projects-overview-grid">
{% assign projects = site.projects | sort: "order" %}
{% for project in projects %}
  <a class="project-tile compact-project-tile" href="{{ project.url | relative_url }}">
    <img src="{{ project.image | relative_url }}" alt="{{ project.image_alt | default: project.title }}" />
    <div class="project-tile-body">
      <div class="project-tile-title">{{ project.title }}</div>
    </div>
  </a>
{% endfor %}
</div>
