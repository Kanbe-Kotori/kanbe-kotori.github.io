---
layout: page
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
  {%- assign date_format = "%Y-%m-%d" -%}
  {% for post in site.posts_diaries %}
    <span class="post-meta">{{ post.date | date: date_format }}</span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>
    </h3>
  {% endfor %}
</ul>
