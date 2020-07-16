---
layout: page
title: About Me
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

<ul class="projects-list">
  {% assign sorted_projects = site.data.projects %}
  {% for project in sorted_projects %}
  <li class="project-item">
    <span class="status {{ project.status | downcase }}">{{ project.status }}</span>
    {% if project.link %}
      <strong><a href="{{ project.link }}" target="_blank">{{ project.id }}</a></strong>
    {% else %}
      <strong>{{ project.id }}</strong> 
    {% endif %}
    {{ project.description }}
  </li>
  {% endfor %}
</ul>
