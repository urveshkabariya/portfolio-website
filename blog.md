---
layout: page
title : Blog
header : Post Archive
group: navigation
---

<div id="blog">

  {% include JB/setup %}
  {% assign posts_collate = site.posts %}
  {% include JB/posts_collate %}

</div>
