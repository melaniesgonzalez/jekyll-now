---
layout: default
title: Jekyll Postings
---

<link rel="stylesheet" href="index.css" />

{% for album in site.postings reversed %}
  <article>
    <a href="{{ postings.url }}">
      <img src="{{ postings.img }}" alt="{{ postings.title }} {{ postings.artist }}"/>
      <p>{{ postings.title }}</p>
    </a>
    <p>by {{ postings.artist }}</p>
  </article>
{% endfor %}

