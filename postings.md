---
layout: default
---

<link rel="stylesheet" href="index.css" />

<div class="posts">
  {% for posting in site.postingss %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ posting.url }}">{{ posting.title }}</a></h1>
      <div class="entry">
        {{ posting.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ posting.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
