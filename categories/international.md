---
layout: default
title: 国際
permalink: /categories/international/
---

<ul class="post-list">
  {% for post in site.categories.international %}
    <li class="post-card">

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
