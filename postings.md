---
layout: default
title: Jekyll Postings
---

<link rel="stylesheet" href="index.css" />

{% for postings in site.postings %}

   <article>
      <a href="{{ postings.url | prepend: site.baseurl }}">
         <p>{{ postings.title }}</p>
      </a>
      <p class="post-excerpt">{{ postings.description | truncate: 160 }}</p>
   </article>
{% endfor %}      
