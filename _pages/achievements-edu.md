---
layout: page
permalink: /educational
title: Achievements
description: A list of achievements
nav: false
display_categories: [Educational, International, Individual, National]
---

<!-- pages/projects.md -->
<div class="projects">
  {% for category in page.display_categories %}
  <a id="{{ category }}" href="{{ site.url }}/achievements/#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>

  {% assign limit = 2 %}
  {% assign categorized_achievements = site.achievements | where: "category", category %}
  {% assign size = categorized_achievements.size %}
  {% if category == "Educational" %}
    {% assign limit = 100 %}
  {% endif %}
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
