---
title: Bebés en movimiento
layout: default
---

<div class="movement-banner-container">
  <div class="title-container">
    <h1>{{ site.data.movement.title}}</h1>
    <span>{{ site.data.movement.highlight }}</span>
  </div>
</div>
<div class="movement-content-container">
  <div class="summary">
    <p>{{ site.data.movement.summary }}</p>
  </div>
  <div class="main-image">      
  </div>
  <div class="highlight-phrase">
    <p>{{ site.data.movement.mainPhrase }}</p>
    <span>{{ site.data.movement.mainPhraseAuthor }}</span>
  </div>    
</div>
  
<div class="services-container">
  <div class="title-container">
    <h1>
      {{ site.data.movement.subTitle }}
    </h1>
  </div>
  <div class="services">
    {% for service in site.data.movement.services %}
    <div class="{{ service.service.type }}">
      <h1>{{ service.service.name }}</h1>      
    </div>
    {% endfor %}
  </div>
</div>
<div class="quote-container">
  {% for quote in site.data.movement.quotes %}
  <div class="highlight-phrase">
    <p>{{ quote.quote }}</p>
    <span>{{ quote.author }}</span>
  </div> 
  {% endfor %}
</div>
