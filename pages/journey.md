---
layout: page
title: Journey
permalink: /pages/journey/
---

<div class="journey-grid">
{% for story in site.journey %}
<div class="journey-card">
  {% if story.image %}
  <img src="{{ story.image | relative_url }}" alt="{{ story.title }}" loading="lazy">
  {% endif %}
  <div class="journey-card-body">
    <h3>{{ story.title }}</h3>
    <div class="journey-date">{{ story.date_label }}</div>
    <p>{{ story.summary }}</p>
  </div>
</div>
{% endfor %}
</div>
