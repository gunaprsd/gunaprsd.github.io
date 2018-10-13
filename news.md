---
layout: default
title: Guna Prasaad | News
---
<h2>News</h2>
<ul class="news">
  {% assign news = (site.data.news | sort: 'date') | reverse %} {% for n in news %}
  <li><span>{{ n.date | date: "%B %-d, %Y" }}</span> {{ n.description | markdownify }} </li>
  {% endfor %}
</ul>


