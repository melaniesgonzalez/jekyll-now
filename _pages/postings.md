---
layout: default
title: Jekyll Postings
---

{% for themes in site.postings %}


<a href="{{ postings.url | prepend: site.baseurl }}">
        <h2>{{ postings.title }}</h2>
</a>

<p class="post-excerpt">{{ postings.description | truncate: 160 }}</p>

{% endfor %} 
