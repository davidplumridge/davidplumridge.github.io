---
layout: page
title: About Me
order: 1
---

Hi, I'm a Full Stack Dev, Architect & Founder.

### Projects

Here are some of my recent [projects](/projects)

### Blog

Here are some recent blogs:

<div class="home">
    <ul>
      {%- assign recent_posts = site.posts | limit: 5 -%}
      {%- for post in recent_posts -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a> - <span>{{ post.date | date: date_format }}</span>
        {%- if site.show_excerpts -%}
          <p>{{ post.excerpt }}</p>
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>
</div>

To see all my blogs, click [here](/blog)
