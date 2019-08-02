---
title: "2018-2019年受打壓工運人士"
lang: zht
lang-ref: activists
permalink: "/activists-zht.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">
            
            
        {% for post in site.tags.activists-zht %}
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
