---
title: "快訊"
lang: zht
lang-ref: news
permalink: "/news-zht.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">

            
        {% for post in site.tags.news-zht %}
        {% if post.title != null %}
          {% if group == null or group == post.group %}
         
            {% include main-loop-card.html %}
          {% endif %}
        {% endif %}
        {% endfor %}
        {% assign group = nil %}
        

        </div>
        
    </div>
</div>
