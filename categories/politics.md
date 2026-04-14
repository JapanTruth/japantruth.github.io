---
layout: default
title: 政治
permalink: /categories/politics/
---

<ul class="post-list">
  {% for post in site.categories.politics %}
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
