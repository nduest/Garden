---
layout: default
title: Links
permalink: /links
---

<div>
  <h1 class="post-title">All links</h1>

  {% for link in site.data.links %}
  
  <div class="list-entry">
    <div><a target="_blank" rel="noopener" href="{{ link.url }}">{{ link.name }}</a> <span class="faded">({{ link.date | date: "%Y-%m-%d" }})</span></div>
    <div>{{ link.description_html }}</div>
  </div>
  {% endfor %}
</div>
