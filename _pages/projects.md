---
layout: default
title: Gabe Elkachouty – Portfolio
permalink: /projects/
---

<div class="gallery-container">
  <div class="project-gallery">

    {% for project in site.projects %}
      {% if project.title and project.url and project.image %}
        <div class="gallery-item">
          <a href="{{ project.url | relative_url }}">
            <img
              src="{{ project.image | relative_url }}"
              alt="{{ project.title }}"
            />
            <p>
              {{ project.display_title | default: project_
