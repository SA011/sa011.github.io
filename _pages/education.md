---
layout: page
permalink: /education/
title: Education
description: 
nav: true
nav_order: 5
---

<div>
  {% assign education = site.education %}
  {% assign size = education.size %}
  {% if education %}
    <div class="container">
      <div class="row row-cols-1 row-cols-md-1">
      {% for content in education %}
        {% if content.visible != false %}
          {% include education.liquid %}
        {% endif %}
      {% endfor %}
      </div>
    </div>
  {% endif %}


</div>
