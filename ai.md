---
layout: page
title: Artificial Intelligence
---

{% for tag in site.tags %}
  {% if tag[0] == "ai" %}
  <h3>Artificial Intelligence</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
  {% endif %}
{% endfor %}
