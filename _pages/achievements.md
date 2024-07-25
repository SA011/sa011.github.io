---
layout: page
permalink: /achievements/
title: Achievements
description: 
nav: true
nav_order: 2
display_categories: [International, Individual, National, Educational]
show_more: false
---

<!-- pages/projects.md -->
<div class="projects">
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>

  {% assign limit = 2 %}
  {% if page.show_more == false %}
    {% assign limit = 100 %}
  {% endif %}
  {% assign categorized_achievements = site.achievements | where: "category", category %}
  {% assign size = categorized_achievements.size %}
  {% if categorized_achievements %}
    {% assign sorted_achievements = categorized_achievements | sort: "importance" %}
    <div class="container">
      <div class="row row-cols-1 row-cols-md-1">
      {% for achievement in sorted_achievements %}
        {% if achievement.visible != false and achievement.importance <= limit %}
          {% include achievements.liquid %}
        {% endif %}
      {% endfor %}
      </div>
    </div>
    {% if size > limit %}
      <center><a href="{{ site.url }}/{{ category | downcase }}">Show more</a></center>
    {% endif %}

  {% endif %}

  {% endfor %}

</div>
