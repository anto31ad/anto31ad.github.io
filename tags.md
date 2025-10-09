---
layout: page
title: "Topics"
permalink: "/topics/"
---

<ul>
{% for tag in site.tags %}
  <li>
    <strong>{{ tag[0] }}</strong>:
    {% for post in tag[1] %}
      <a href="{{ post.url }}">{{ post.title }}</a>{% unless forloop.last %}, {% endunless %}
    {% endfor %}
  </li>
{% endfor %}
</ul>