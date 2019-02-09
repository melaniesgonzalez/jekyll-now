---
layout: default
title: Jekyll Postings
---

<link rel="stylesheet" href="index.css" />

<ul>
  {% for posting in site.postings reversed %}
    <article>
      <a href="{{ postings.url }}">{{ postings.title }}</a>
      - {{ postings.description }}
    </article>
  {% endfor %}
</ul>
