---
title: "2018-2019年受打压工运人士"
lang: zh
lang-ref: activists
permalink: "/activists-zh.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">
            
            
        {% for post in site.tags.activists-zh %}
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
