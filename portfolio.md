---
layout: default
---

{% for portfolio in site.portfolio %}
   <article>
      <a href="{{ portfolio.url | prepend: site.baseurl }}">
         <p>{{ portfolio.title }}</p>
      </a>
      <p class="portfolio-excerpt">{{ portfolio.description | truncate: 160 }}</p>
   </article>
{% endfor %}     
