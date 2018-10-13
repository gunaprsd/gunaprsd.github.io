---
layout: default
title: Guna Prasaad | News
---
<h3>News</h3>
<table class="news">
  <col width="30%">
  <col width="70%">
  {% assign news = (site.data.news | sort: 'date') | reverse %} {% for n in news %}
  <tr>
    <td> <span class="date">{{ n.date | date_to_string }} &raquo; </span> </td> 
    <td> {{ n.description | markdownify }} </td>
  </tr>
  {% endfor %}
</table>


