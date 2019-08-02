---
title: "Take Action"
lang: en
lang-ref: support
permalink: "/support.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">

            
        {% for post in site.tags.support %}
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
