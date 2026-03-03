---
layout: page
title: Projects
permalink: /pages/projects/
---

<div class="project-grid">
{% for project in site.projects %}
<div class="project-card">
  <h3>{{ project.title }}</h3>
  <div class="project-period">{{ project.period }}</div>
  <p>{{ project.description }}</p>
  {% if project.tech %}
  <div class="project-tech">
    {% for t in project.tech %}<span class="tag">{{ t }}</span>{% endfor %}
  </div>
  {% endif %}
</div>
{% endfor %}
</div>
