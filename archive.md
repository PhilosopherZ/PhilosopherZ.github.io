---
layout: page
title: "Archive"
description: "泰山不让土壤，故能成其大；河海不择细流，故能就其深"
header-img: "img/reading-books.jpg"
---


<ul class="listing">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <h1 class="listing-seperator">{{ y }}年</h1>
  {% endif %}
  {% capture mon %}{{post.date | date:"%m"}}{% endcapture %}
  {% if month != mon %}
    {% assign month = mon %}
    <h3 class="listing-seperator">{{ mon }}月</h3>
  {% endif %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
