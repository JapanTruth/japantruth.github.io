---
layout: default
title: 投資
permalink: /categories/investment/
---

<h1>投資</h1>

{% for post in site.categories.investment %}
  <div>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  </div>
{% endfor %}
