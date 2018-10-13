---
layout: default
title: Guna Prasaad | News
---
<h2>News</h2>
<p>
<ul class="posts">
  {% assign news = (site.data.news | sort: 'date') | reverse %} {% for n in news %}
  <li><span> {{ n.date | date_to_string }} &raquo; </span> {{ n.description | markdownify }}</li>
  {% endfor %}
</ul>
</p>

