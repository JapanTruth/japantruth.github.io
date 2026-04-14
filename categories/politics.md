---
layout: default
title: 政治
permalink: /categories/politics/
---

<h1></h1>

{% for post in site.categories.politics %}
  <div>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  </div>
{% endfor %}
