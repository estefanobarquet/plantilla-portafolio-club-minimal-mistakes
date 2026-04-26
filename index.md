---
layout: home
author_profile: true
header:
  overlay_image: /assets/images/header-banner.jpg
  overlay_filter: 0.5
  title: "Estefano Farid Barquet Vera"
  excerpt: "Toward Fully Autonomous Mobile Robot System"

feature_row:
  - image_path: /assets/images/project1-thumb.jpg
    title: "Extension to Multi-Agent!"
    excerpt: "Distributed multi-agent target tracking."
    url: "/projects/project-1/"
  - image_path: /assets/images/project2-thumb.jpg
    title: "Super Efficient Planning!"
    excerpt: "Bernstein polynomial motion primitive-based tracking."
    url: "/projects/project-2/"
  - image_path: /assets/images/project3-thumb.jpg
    title: "Learning-based Tracking!"
    excerpt: "Target tracking using CM-VAE."
    url: "/projects/project-3/"
---

Hi, I am Estefano, a **robotics engineering student**. My research interests are Autonomous Navigation and Computer Vision.

You can see my works through these links: [RESEARCH](/research/) and [PROJECTS](/projects/)

{% include feature_row %}

<hr>


<div class="entries-list">
  {% for post in site.posts limit:5 %}
    {% if post.categories contains 'publications' %}{% continue %}{% endif %}
    <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork" style="display: flex; align-items: flex-start; margin-bottom: 1.5em;">
      <div class="archive__item-teaser" style="flex: 0 0 200px; margin-right: 20px;">
        <img src="{{ post.header.teaser | relative_url }}" alt="" style="width: 100%; border-radius: 4px;">
      </div>
      <div class="archive__item-body">
        <h2 class="archive__item-title no_toc" itemprop="headline" style="margin-top: 0; font-size: 1.2em;">
          <a href="{{ post.url | relative_url }}" rel="permalink">{{ post.title }}</a>
        </h2>
        <p style="font-size: 0.85em; color: #666;">{{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    </article>
  {% endfor %}
</div>