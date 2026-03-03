---
layout: page
title: Knowledge Gradient Ascent
permalink: /pages/blog/
---

<ul class="post-list">
{% for post in site.posts %}
<li class="post-list-item">
  <h2 class="post-list-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <div class="post-list-meta">
    {{ post.date | date: "%B %d, %Y" }}
    {% if post.tags.size > 0 %} &middot;
    {% for tag in post.tags %}<span class="tag">{{ tag }}</span> {% endfor %}
    {% endif %}
  </div>
  {% if post.excerpt %}
  <p class="post-list-excerpt">{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
  {% endif %}
</li>
{% endfor %}
</ul>

{% if site.posts.size == 0 %}
<p>Posts coming soon. Stay tuned!</p>
{% endif %}
