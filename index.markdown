---
title: Créate es
layout: default
---
<div class="home-banner">
  <div>
    <h1>{{ site.data.home.banner.title }}</h1>
    <h2>{{ site.data.home.banner.subTitle }}</h2>
  </div>
</div>

<div class="home-content">
  <div class="title-container">
    <h1>
      {{ site.data.home.title }}
    </h1>
  </div>
  <div class="bullet-container">
    <div class="bullets">
      <ul>
      {% for item in site.data.home.content.bullets %}
          <li>{{ item }}</li>
      {% endfor %}
      </ul>
    </div>
    <div class="bullet-photo">
    </div>
  </div>
</div>

<div class="services-container">
  <div class="title-container">
    <h1>
      {{ site.data.home.serviceArea.title }}
    </h1>
  </div>
  <div class="services">
    {% for service in site.data.home.serviceArea.services %}
    <div class="{{ service.service.type }}">
      <h1>{{ service.service.name }}</h1>      
    </div>
    {% endfor %}
  </div>
</div>