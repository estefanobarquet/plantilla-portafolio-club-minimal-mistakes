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
  {% for post in site.categories.projects %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>