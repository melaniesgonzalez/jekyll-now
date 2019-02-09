---
layout: default
title: Jekyll Postings
---

<link rel="stylesheet" href="index.css" />

{% for postings in site.postings %}


<a href="{{ postings.url | prepend: site.baseurl }}">{{ postings.title }}

</a>

<p class="post-excerpt">{{ postings.description | truncate: 160 }}</p>

{% endfor %}      
