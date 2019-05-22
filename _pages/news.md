---
title: "News"
permalink: "/news.html"
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-8">

            
        {% for post in site.tags.news %}
        {% if post.title != null %}
          {% if group == null or group == post.group %}
         
            {% include main-loop-card.html %}
          {% endif %}
        {% endif %}
        {% endfor %}
        {% assign group = nil %}
        

        </div>
        
            <div class="col-md-4">
        {% include sidebar-featured.html %}    
    </div>
        
    </div>
</div>
