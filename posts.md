---
layout: page
title: "Posts"
permalink: "/posts/"
---

<ul>
  {% for post in site.posts %}
    <li>
      {% if post.lang == "it" %}🇮🇹
      {% else post.lang == "en" %}🇬🇧
      {% endif %}
      <a href="{{ post.url }}">{{ post.title }} ({{ post.date | date: "%Y-%m-%d" }})</a>
    </li>
  {% endfor %}
</ul>
