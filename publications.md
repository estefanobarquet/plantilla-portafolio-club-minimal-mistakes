---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
header:
  overlay_image: /assets/images/header-banner.jpg
  overlay_filter: 0.5
---

## Under review

{% assign under_review = site.posts | where_exp: "post", "post.categories contains 'publications'" | where: "pub_status", "review" %}
{% for post in under_review %}
{{ post.content }}
{% endfor %}

## Papers

{% assign papers = site.posts | where_exp: "post", "post.categories contains 'publications'" | where: "pub_status", "paper" %}
{% for post in papers %}
{{ post.content }}
{% endfor %}