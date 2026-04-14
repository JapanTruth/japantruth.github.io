---
layout: default
title: 投資
permalink: /categories/investment/
---

<ul class="post-list">
  {% for post in site.categories.investment %}
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
