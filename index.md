---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: about me
order: 1
---

I'm a full stack developer / architect. I like to build things and occasionally write a blog about it.

Check out some of my recent <a class="page-link" href="/projects">projects</a>. You can contact me <a class="page-link" href="/contact">here</a>.

# Blogs

(I'm still migrating some of my blogs onto this site)

<div class="home">

  {%- if site.posts.size > 0 -%}
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
  {%- endif -%}

</div>