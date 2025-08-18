---
layout: page
title: David Plumridge | Developer, Architect & Founder
heading: About me
description: David Plumridge - Full Stack Developer, Cloud Architect & Startup Founder. Building innovative solutions with modern web technologies.
order: 1
---

Hi there! I'm a Full Stack Developer, Cloud Architect, and Startup Founder 🚀 👨‍💻 ✨

### 🤝 Connect with me ...
<ul class="social-links">
  {% for social in site.data.socials %}
    <li>
      <a href="{{ social.href }}" target="_blank" title="Connect on {{ social.id }}">
        <i class="fa {{ social.fa-icon }}"></i>
        {{ social.id }}
      </a>
    </li>
  {% endfor %}
</ul>

### 🚧 My projects ...

<div class="projects-container">
  <ul class="projects-list">
    {% assign sorted_projects = site.data.projects %}
    {% for project in sorted_projects %}
    <li class="project-item">
      {% if project.link %}
        <a href="{{ project.link }}" target="_blank" class="project-card-link">
      {% else %}
        <div class="project-card-link no-link">
      {% endif %}
        <div class="project-card">
          {% if project.status contains '🚀' %}
            <span class="status-badge active">🚀 ACTIVE</span>
          {% elsif project.status contains '💰' %}
            <span class="status-badge sold">💰 SOLD</span>
          {% elsif project.status contains '☠️' %}
            <span class="status-badge inactive">☠️ INACTIVE</span>
          {% endif %}
          <div class="project-details">
            <div class="project-title">{{ project.id }}</div>
            <div class="project-description">{{ project.description }}</div>
          </div>
        </div>
      {% if project.link %}
        </a>
      {% else %}
        </div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
