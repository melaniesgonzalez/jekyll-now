---
layout: default
---

{% for portfolio in site.portfolio %}
   <article>
      <a href="{{ portfolio.url | prepend: site.baseurl }}">
         <p>{{ portfolio.title }}</p>
      </a>
      <p class="post-excerpt">{{ portfolio.description | truncate: 160 }}</p>
      <a href="{{ site.baseurl }}{{ portfolio.url }}" class="read-more">Read More</a>
   </article>
{% endfor %}     
