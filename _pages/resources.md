---
title: "Resources"
lang: en
lang-ref: resources
permalink: "/resources.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">

            
        {% for post in site.tags.resources %}
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
