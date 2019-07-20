---
title: "Victims of the 2018-2019 Labor Crackdown"
lang: en
lang-ref: activists
permalink: "/activists.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">
            
            
        {% for post in site.tags.activists %}
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
