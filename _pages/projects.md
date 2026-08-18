---
layout: page
title: Proyectos
permalink: /projects/
nav: true
nav_order: 2
---

<div class="projects">
  {% assign projects = site.projects | sort: "importance" %}
  {% for project in projects %}
    {% include projects.liquid project=project %}
  {% endfor %}
</div>
