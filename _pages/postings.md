---
layout: default
title: Jekyll Postings
---

<br />

<h1 style="text-align:center">Postings</h1>
<div id="mainbox">
   
     {% for postings in site.postings reversed  %}
       <a class="post-link-index" href="{{ postings.url | prepend: site.baseurl }}">
          <div class="card">
                <img alt="{{ postings.title }}" class="post-image-index" itemprop="thumbnailUrl" src="/thumbs/{{ postings.img }}" width="300" height="auto" />
                <div class="card-footer">
                    <h6 class="post-index-title">{{ postings.title }}</h6>
                <p class="post-excerpt">{{ postings.desc | truncate: 160 }}</p>
               </div>
     
        </div> 
     </a>
      {% endfor %}   
</div>
