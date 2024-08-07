---
layout: page
title: About Me
order: 1
---

Hi, I'm a Full Stack Dev, Architect & Founder 🚀👨‍💻

### 🚧 Projects

Some of the things I've been working on:

<ul>
  {% for project in site.data.projects | limit: 50 -%}
  <li class="list-item">
    {% if project.link %}
      <strong><a href="{{ project.link }}" target="_blank">{{ project.id }}</a></strong>
    {% else %}
      <strong>{{ project.id }}</strong> 
    {% endif %}
    <span class="status {{ project.status | downcase }}">{{ project.status }}</span>
    {{ project.description }}
  </li>
  {%- endfor -%}
</ul>

### ✍️ Blog

Here's some blogs I've written (without chat GPT):

<ul>
  {%- for post in site.posts | limit: 50 -%}
  <li class="list-item">
    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>: {{ post.excerpt }}
  </li>
  {%- endfor -%}
</ul>

### 🤝 Connect with me

Want to say hello? Reach me at:

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
