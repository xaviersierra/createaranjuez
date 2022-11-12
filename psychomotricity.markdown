---
title: Psicomotricidad Vivenciada
layout: default
---
{% include content-page.html data=site.data.psychomotricity name="phychomotricity" %}

<div class="phychomotricity-note-container">
    <div class="note-image">
    </div>
    <div class="note-text">
        <h1>
            {{ site.data.psychomotricity.notes.title }}
        </h1>
        {% for note in site.data.psychomotricity.notes.texts %}
        <p>
            {{ note }}
        </p>
        {% endfor %}
    </div>
</div>
{% include services.html services=site.data.psychomotricity.services title=site.data.psychomotricity.serviceTitle %}