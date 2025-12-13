---
layout: default
title: <Priya Abiram> - Portfolio
permalink: /projects/
---

<div class="container mt-5">
  <h1 class="text-center mb-4">My Projects</h1>
  <div class="row">
    {% for project in site.projects %}
      <div class="col-md-6 col-lg-4 mb-4">
        <div class="card h-100 shadow-sm">
          <div class="card-body d-flex flex-column">
            <h5 class="card-title">{{ project.title }}</h5>
            <p class="card-text flex-grow-1">{{ project.content | strip_html | truncate: 100 }}</p>
            <a href="{{ project.url | relative_url }}" class="btn btn-primary mt-auto">View Project</a>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
</div>