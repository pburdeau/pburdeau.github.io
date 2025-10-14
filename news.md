---
title: "News"
permalink: /news/
layout: single
---

<ul>
{% assign items = site.news | sort: 'date' | reverse %}
{% for item in items %}
  <li><a href="{{ item.url }}">{{ item.title }}</a> <small>— {{ item.date | date: "%b %d, %Y" }}</small></li>
{% endfor %}
</ul>