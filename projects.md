---
layout: page
title: Projects
order: 2
---

<div class="projects">
  {% for project in site.data.projects %}
    <div class="project">
      <div class="project-icon"><i class="{{ project.icon }}"></i></div> <!-- Use FontAwesome icon here -->
      <div class="project-content">
        <h2>{{ project.id }} <span class="status">({{ project.status }})</span></h2>
        {% if project.tech %}
          <p><strong>Tech:</strong> {{ project.tech }}</p>
        {% endif %}
        <p>{{ project.description }}</p>
        {% if project.link %}
          <p><a href="{{ project.link }}" target="_blank">{{ project.link-text }}</a></p>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
