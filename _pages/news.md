---
layout: page
title: News
permalink: /News/
nav: true
nav_order: 5
---

<ul class="news-list">
{% assign sorted_news = site.news | sort: "date" | reverse %}

{% for item in sorted_news %}
  <li class="news-item">
    <span class="news-date">
      {{ item.date | date: "%b %d, %Y" }}
    </span>

    <div class="news-content">
      {{ item.content }}
    </div>
  </li>
{% endfor %}
</ul>
