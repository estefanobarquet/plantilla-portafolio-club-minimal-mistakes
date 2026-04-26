---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
header:
  overlay_image: /assets/images/header-banner.jpg
  overlay_filter: 0.5
---

<div class="entries-list">
  {% assign project_posts = site.posts | where: "categories", "projects" %}
  {% for post in project_posts %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>