---
layout: splash
title: "code & programming"
---
{% include JB/setup %}

##1 - Python

<ul class="thumbnails">
  {% assign pages_icons = site.posts %}
  {% assign pages_category = "learning" %}
  {% assign pages_tag = "python" %}
  {% include custom/pages_cat_tag %}
</ul>

##2 - Java

<ul class="thumbnails">
  {% assign pages_icons = site.posts %}
  {% assign pages_category = "learning" %}
  {% assign pages_tag = "java" %}
  {% include custom/pages_cat_tag %}
</ul>

##3 - 开发辅助

<ul class="thumbnails">
  {% assign pages_icons = site.categories.tool %}
  {% include custom/pages_reversed %}
</ul>
