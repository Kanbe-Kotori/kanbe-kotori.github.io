---
layout: collection
title: 日寄
---

<div class="post-content">
  <h2>写在前面</h2>
</div>

<ul class="post-list">
  <span class="post-meta">手动置顶</span>
  <h3>
    <a class="post-link" href="./about">关于本页</a>
  </h3>
</ul>

---

<div class="post-content">
  <h2>时间线</h2>
</div>

<ul class="post-list">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
  {% for post in site.categories.diaries %}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
      {%- if site.show_excerpts -%}
        {{ post.excerpt }}
      {%- endif -%}
    </li>
  {% endfor %}
</ul>
