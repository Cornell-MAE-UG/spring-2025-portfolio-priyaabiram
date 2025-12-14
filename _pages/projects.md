---
layout: default
title: <Priya Abiram> - Portfolio
permalink: /projects/
---

<section class="section">
  <div class="section-header">
    <h1>My Projects</h1>
    <p>Selected coursework and extracurricular projects spanning flight hardware, ethics analysis, systems integration, and outreach.</p>
  </div>
  <div class="card-grid">
    {% for project in site.projects %}
      {% assign card_image = project.image | default: site.default_project_image | default: '/assets/images/function-graph.png' %}
      {% assign summary_source = project.summary | default: project.description | default: project.excerpt %}
      <article class="project-card">
        {% if card_image %}
          <img src="{{ card_image | relative_url }}" alt="{{ project.title }} cover image" class="img-fluid rounded mb-3">
        {% endif %}
        <h5>{{ project.title }}</h5>
        <p class="text-muted">{{ summary_source | strip_html | truncate: 120 }}</p>
        <a href="{{ project.url | relative_url }}" class="btn btn-primary btn-icon">View project <i class="bi bi-arrow-right"></i></a>
      </article>
    {% endfor %}
  </div>
</section>
