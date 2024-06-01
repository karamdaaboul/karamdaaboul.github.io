---
layout: home
title: Committed Towards a Better Future
listing:
  contents: posts
  sort: "date desc"
  type: default
  categories: true
  sort-ui: true
  filter-ui: false
page-layout: full
title-block-banner: true
---

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
  <a href="{{ post.url }}">Read more...</a>
{% endfor %}
