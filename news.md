---
layout: default
title: Guna Prasaad | News
---
<h3>News</h3>
<table class="news">
  <tr>
    <th style="width:30%"></th>
    <th style="width:70%"></th>
  </tr>
  {% assign news = (site.data.news | sort: 'date') | reverse %} {% for n in news %}
  <tr>
    <td class="date">{{ n.date | date_to_string }} &raquo; </td> 
    <td> {{ n.description | markdownify }} </td>
  </tr>
  {% endfor %}
</table>


