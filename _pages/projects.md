---
layout: default
title: <Priya Abiram> - Portfolio
permalink: /projects/
---

<div class="container mt-5">
  <h1 class="text-center mb-4">My Projects</h1>
  <ul class="list-group">
    {% for project in site.projects %}
      <li class="list-group-item">
        <a href="{{ project.url | relative_url }}" class="text-decoration-none">
          <h5 class="mb-1">{{ project.title }}</h5>
        </a>
        <p class="mb-1">{{ project.content | strip_html | truncate: 150 }}</p>
      </li>
    {% endfor %}
  </ul>
</div>