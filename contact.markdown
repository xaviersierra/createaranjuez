---
title: Contacto
layout: default
---

<div class="contact-container content-container">
    <div class="title-container">
        <h1>
            {{ site.data.contact.title }}
        </h1>
    </div>
    <div class="contact-content">
        <div class="content">
            <div class="description">
                {{ site.data.contact.contentDescription }}
            </div>
            <div class="location-container">
                <div class="title-container">
                    <h2>{{ site.data.contact.location.title }}</h2>
                </div>
                <div class="address">
                    {% for line in site.data.contact.location.address %}
                    <p>{{ line }}</p>
                    {% endfor %}
                </div>
            </div>
            <div class="email-container">
                <div class="title-container">
                    <h2>{{ site.data.contact.email.title }}</h2>
                </div>
                <div class="email">
                    <p>{{ site.data.contact.email.email }}</p>
                </div>
            </div>
            <div class="phone-container">
                <div class="title-container">
                    <h2>{{ site.data.contact.phones.title }}</h2>
                </div>
                <div class="phone">
                {% for phone in site.data.contact.phones.phones %}
                <ul>
                    <li>
                        <span class="name">{{ phone.name }}</span>
                        -
                        <span class="number">{{ phone.number }}</span>
                    </li>                    
                </ul>
                {% endfor %}
                </div>
            </div>
        </div>
        <div class="contact-banner">
        </div>
    </div>
</div>