---
layout: page
title: 分类
permalink: /categories/
---

<ul>
  {% for category in site.categories %}
    <li>
      <a class="category-post-title" href="{{ site.baseurl }}/categories/{{ category[0] | slugify }}/">
        {{ category[0] }} ({{ category[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>

<style>
.category-post-title {
  font-size: 1.5em;
  font-weight: bold;
  display: inline-block;
  margin-bottom: 4px;
}
</style>