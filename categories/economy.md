---
layout: default
title: 経済
permalink: /categories/economy/
---
<ul class="post-list">
  {% for post in site.categories.economy %}
    <li class="post-card">
      {% if post.image %}
      <img src="{{ post.image }}" alt="{{ post.title }}">
      {% endif %}
      <div class="post-date">
        {{ post.date | date: "%Y.%m.%d" }}
      </div>
      <h2>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </h2>
      <p class="excerpt">
        {{ post.excerpt | strip_html | truncate: 120 }}
      </p>
    </li>
  {% endfor %}
</ul>
