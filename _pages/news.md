---
layout: page
title: News
permalink: /News/
nav: true
nav_order: 5
---

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
