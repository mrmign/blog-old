---
layout: splash
title: "学习笔记"
---
{% include JB/setup %}

##0 - C,C++
<ul class="thumbnails">
  {% assign pages_icons = site.tags.c %}
  {% include custom/pages_reversed %}
</ul>

##1 - Python

<ul class="thumbnails">
  {% assign pages_icons = site.tags.python %}
  {% include custom/pages_reversed %}
</ul>

## 2 - 学习Jekyll

<ul class="thumbnails">
  {% assign pages_icons = site.tags.jekyll %}
  {% include custom/pages_reversed %}
</ul>


##3 - 开发辅助

<ul class="thumbnails">
  {% assign pages_icons = site.categories.tool %}
  {% include custom/pages_reversed %}
</ul>