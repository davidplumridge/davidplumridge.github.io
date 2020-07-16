---
layout: page
title: About Me
---

Full stack developer & architect.

I like building things, here are some of my <a href="/projects">projects</a>.

Occasionally, I write a blog about something random: 

<div class="home">
    <ul>
      {%- for post in site.posts -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>
</div>