---
layout: page
title: Blog
order: 3
---

Here is a list of all my blog posts:

<div class="archive">
    <ul>
      {%- for post in site.posts -%}
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
