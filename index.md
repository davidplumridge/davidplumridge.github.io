---
layout: page
title: About Me
order: 1
---

Hi, I'm a Full Stack Dev, Architect & Founder 🚀👨‍💻

### 🚧 My projects ...

<ul style="list-style-type: none;">
  {% assign sorted_projects = site.data.projects %}
  {% for project in sorted_projects %}
  <li class="list-item">
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
