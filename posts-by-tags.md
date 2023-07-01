---
layout: page
title: Posts by Tags
---
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
              {% assign full_url = site.url | append: '/notes' | append: post.url %}
	      {{ full_url }}

          <li><a href="{{ full_url }}">{{ post.title }}</a>, published {{ post.date | date: "%Y-%m-%d" }}</li>
    {% endfor %}
  </ul>
{% endfor %}