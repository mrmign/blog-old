---
layout: landing
title: Arming's blog!
head_title:
description: Record of my learning.
---

<div class="row" style="margin-bottom:20px;">
  <div style="width:100%">
    <h3 style="margin-bottom:5px; margin-left:20px; color:#333333;">The dog equally study, the gentleman equally plays.</h3>
    <!--
    <h6 align="right" style="font-size:12px; margin-right:8px">喜欢我或者我的博客，可以把它加入你的<a href="javascript:void(0)" onclick="window.external.AddFavorite(location.href, document.title)">收藏夹</a></h6>
  -->
  </div>
  <div class="divbox" style="width:96%;margin-right:0px;padding-right:10px;">
    <h1 id="start-now" style="margin-left: 0px; margin-right: 0px; font-size: 22px;">The Latest Blogs</h1>
    <div style="margin-left:-15px">
    {% assign posts_all = site.posts %}
    {% assign count = 10 %}
    {% include custom/posts_all %}
  </div>
  </div>
  
</div>

