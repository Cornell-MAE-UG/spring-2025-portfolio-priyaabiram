---
layout: default
title: <Priya Abiram> - Portfolio
permalink: /projects/
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <p>{{ project.title}}</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>