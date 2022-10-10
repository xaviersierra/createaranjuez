---
title: Sobre nosotras
layout: default
---

<div class="about-us-container">
  <div class="title-container">
    <h1>{{ site.data.about.title }}</h1>
    <p>{{ site.data.about.summary}}</p>
  </div>
  <div>
     <img alt="group picture">
  </div>
</div>
<div class="about-us-content-container">
  <div class="title-container">
    <h1>{{ site.data.about.subTitle}}</h1>
  </div>
  {% for item in site.data.about.us %}
  <div>
    <h2>{{ item.name }}</h2>
    <p>{{ item.description }}</p>
    <span>{{ item.finalThought}}</span>
  </div>
  {% endfor %}  
</div>