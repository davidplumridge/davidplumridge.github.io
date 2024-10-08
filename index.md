---
layout: page
title: About Me
order: 1
---

Hi, I'm a Full Stack Dev, Architect & Founder 🚀👨‍💻

### 🚧 Projects

<ul style="list-style-type: none;">
  {% for project in site.data.projects | limit: 50 -%}
  <li class="list-item">
    <span class="status {{ project.status | downcase }}">{{ project.status }}</span>
    {% if project.link %}
      <strong><a href="{{ project.link }}" target="_blank">{{ project.id }}</a></strong>
    {% else %}
      <strong>{{ project.id }}</strong> 
    {% endif %}
    {{ project.description }}
  </li>
  {%- endfor -%}
</ul>

### ✍️ Blog posts

<ul>
  {%- for post in site.posts | limit: 50 -%}
  <li class="list-item">
    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>: {{ post.excerpt }}
  </li>
  {%- endfor -%}
</ul>

### 🤝 Connect with me

<ul>
  {% for social in site.data.socials %}
    <li class="list-item">
      <a href="{{ social.href }}" target="_blank">
        <i class="fa {{ social.fa-icon }}" style="margin-right: 5px;"></i>
        {{ social.id }}
      </a>
    </li>
  {% endfor %}
</ul>
