---
layout: page
title: Proyectos
permalink: /projects/
nav: true
nav_order: 2
---

<div class="projects">
  {% for project in site.projects %}
    <div class="project-card">
      <h2>
        <a href="{{ project.url | relative_url }}">
          {{ project.title }}
        </a>
      </h2>

      {% if project.description %}
        <p>{{ project.description }}</p>
      {% endif %}

      {% if project.category %}
        <p><small>Categoría: {{ project.category }}</small></p>
      {% endif %}
    </div>
  {% endfor %}
</div>
