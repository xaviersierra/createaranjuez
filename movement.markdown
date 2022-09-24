---
title: Bebés en movimiento
layout: default
---
<div>
  <div>
    <div>
      <h1>{{ site.data.movement.title}}</h1>
      <span>{{ site.data.movement.highlight }}</span>
    </div>
    <div>
      <p>{{ site.data.movement.summary }}</p>
    </div>
    <div>
      <p>{{ site.data.movement.mainPhrase }}</p>
    </div>    
  </div>
  <div>
    {% for service in site.data.movement.services %}
    <div>
      {{ service.name }}
      <img alt="pending">
    </div>
    {% endfor %}
    {% for item in site.data.movement.quotes %}
    <div>
      <p>{{ item.quote }}</p>
      <span>{{ item.author }}</span>
    </div>
    {% endfor %}
  </div>
</div>