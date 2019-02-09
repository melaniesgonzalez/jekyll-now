---
layout: default
title: Jekyll Postings
---




{% for album in site.postings reversed %}
 <link rel="stylesheet" href="index.css" />
 <article>
    <a href="{{ postings.url }}">
      <img alt="{{ postings.title }} {{ postings.artist }}"/>
      <p>{{ postings.title }}</p>
    </a>
    <p>by {{ postings.artist }}</p>
  </article>
{% endfor %}
