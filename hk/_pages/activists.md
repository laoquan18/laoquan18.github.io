---
title: "2018-2019年受打壓工運人士"
lang: hk
lang-ref: activists
permalink: "/activists-hk.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">
            
            
        {% for post in site.tags.activists-hk %}
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
