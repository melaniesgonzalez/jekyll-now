---
layout: default
---

<link rel="stylesheet" href="index.css" />

{% for postings in site.postings %}
   <article class="post">
      <a href="{{ postings.url | prepend: site.baseurl }}">
         <p>{{ postings.title }}</p>
      </a>
      <p class="post-excerpt">{{ postings.description | truncate: 160 }}</p>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
   </article>
{% endfor %}     
