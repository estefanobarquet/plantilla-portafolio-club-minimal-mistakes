---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  overlay_image: /assets/images/header-banner.jpg
  overlay_filter: 0.5
---

<div class="entries-list">
  {% for post in site.categories.research %}
    <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork">
      <div class="archive__item-teaser">
        <img src="{{ post.header.teaser | relative_url }}" alt="">
      </div>
      <h2 class="archive__item-title no_toc" itemprop="headline">
        <a href="{{ post.url | relative_url }}" rel="permalink">{{ post.title }}</a>
      </h2>
      <div class="archive__item-excerpt" itemprop="description">
        {{ post.excerpt | strip_html | truncate: 160 }}
      </div>
    </article>
  {% endfor %}
</div>