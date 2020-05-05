---
layout: default
title: Announcements
date: 2019-07-01 04:30
author: Klahanie
show-title: true
---
<ul>
    {% for doc in site.announcements reversed %}
        <li><a href="{{site.url}}{{ doc.url }}">{{doc.date | date: "[%B %d, %Y]" }} {{ doc.title }}</a></li>
    {% endfor %}
</ul>


