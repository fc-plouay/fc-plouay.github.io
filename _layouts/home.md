---
layout: default
---

<h1>FC Plouay</h1>

<h2>Actualités</h2>
<ul class="post-list">
{%- for post in site.posts -%}
  <li>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h3>
    {%- assign date_format = "%d/%m/%Y" -%}
    <span class="post-meta">{{ post.date | date: date_format | frenchDate }}</span>
  </li>
{%- endfor -%}
</ul>


