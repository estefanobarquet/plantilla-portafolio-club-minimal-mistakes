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
    <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork" style="display: flex; align-items: flex-start; margin-bottom: 2em;">
      <div class="archive__item-teaser" style="flex: 0 0 250px; margin-right: 20px;">
        <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}" style="width: 100%; border-radius: 4px;">
      </div>
      <div class="archive__item-body">
        <h2 class="archive__item-title no_toc" itemprop="headline" style="margin-top: 0;">
          <a href="{{ post.url | relative_url }}" rel="permalink">{{ post.title }}</a>
        </h2>
        <div class="archive__item-excerpt" itemprop="description" style="font-size: 0.9em;">
          {{ post.excerpt | strip_html | truncate: 160 }}
        </div>
      </div>
    </article>
  {% endfor %}
</div>