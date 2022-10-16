---
title: Sobre nosotras
layout: default
---

<div class="about-us-container">
  <div class="title-container">
    <h1>{{ site.data.about.title }}</h1>
    <p>{{ site.data.about.summary}}</p>
  </div>
  <div class="about-us-banner">     
  </div>
</div>
<div class="about-us-content-container">
  <div class="title-container">
    <h1>{{ site.data.about.subTitle}}</h1>
  </div>
  {% for item in site.data.about.us %}
  <div class="about-us-detail">
    <div class="about-us-title">
      <h2>{{ item.name }}</h2>
    </div>
    <div class="about-us-description">
      {% for paragraph in item.description %}
      <p>{{ paragraph }}</p><br>
      {% endfor %}      
    </div>
    <div class="about-us-pic {{ item.class }}">
    </div>
    <div class="about-us-last">
      {{ item.finalThought}}
    </div>    
  </div>
  {% endfor %}  
</div>