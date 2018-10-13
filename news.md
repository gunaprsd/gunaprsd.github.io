---
layout: default
title: Guna Prasaad | News
---
<h2>News</h2>
<ul class="posts">
  {% assign news = (site.data.news | sort: 'date') | reverse %} {% for n in news %}
  <li> <p> <span> {{ n.date | date: "%B %-d, %Y" }} &raquo; </span> {{ n.description | markdownify }} </p> </li>
  {% endfor %}
</ul>


