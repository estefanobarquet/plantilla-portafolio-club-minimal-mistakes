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
    <p>Intentando cargar imagen desde: <b>{{ post.header.teaser }}</b></p>
    <article class="archive__item">
      <div class="archive__item-teaser">
        <img src="{{ post.header.teaser | relative_url }}" alt="Si ves esto, la ruta falló">
      </div>
      <h2>{{ post.title }}</h2>
    </article>
  {% endfor %}
</div>