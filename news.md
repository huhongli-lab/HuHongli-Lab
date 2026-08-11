---
layout: default
permalink: /news/
title: News
description: Lab latest news and updates
nav: true
nav_order: 5
---

# News

<ul class="news-list">
{% for post in site.posts %}
  <li class="news-item">
    <span class="news-date">{{ post.date | date: "%b %d, %Y" }}</span>
    <div class="news-content">
      {{ post.content }}
    </div>
  </li>
{% endfor %}
</ul>
