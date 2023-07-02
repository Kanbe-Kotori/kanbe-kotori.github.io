---
layout: collection
title: 游记
---
<div class="post-content">
  <h2>写在前面</h2>
</div>

<ul class="post-list">
  <span class="post-meta">手动置顶</span>
  <h3>
    <a class="post-link" href="./about">关于本页</a>
  </h3>

  <span class="post-meta">手动置顶</span>
  <h3>
    <a class="post-link" href="./grading">评分标准</a>
  </h3>
</ul>

---

<div class="post-content">
  <h2>游记一览（多图杀猫）</h2>
</div>

<ul class="post-list">
  {%- assign date_format = "%Y-%m" -%}
  {% for post in site.posts_travels %}
    <span class="post-meta">{{ post.date | date: date_format }}</span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>
    </h3>
  {% endfor %}
  
  <span class="post-meta"> 2022-08</span>
  <h3> 伊春（待填） </h3>
  <span class="post-meta"> 2022-08</span>
  <h3> 哈尔滨（待填） </h3>
  
  <span class="post-meta"> 2022-01</span>
  <h3> 珠海（待填） </h3>
  
  <span class="post-meta"> 2021-08</span>
  <h3> 香港（待填） </h3>
</ul>
