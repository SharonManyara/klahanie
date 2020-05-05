---
layout: default
title: Staff
date: 2019-05-19 06:19
author: Klahanie
comments: true
categories: []
---
<img src="{{site.url}}/images/staff/Staff-Group-Shot-larger.jpg" class="img-fluid">

{% for doc in site.staff %}
{% if doc.title != "Staff" %}
<div class="row mb-4">
  <img class="img-thumbnail col-md-3" src="{{site.url}}{{doc.thumbnail}}">
    <div class="col-md-9">
      <h4>
      <a href="mailto:{{doc.email}}">{{doc.title}}</a>
      </h4>
      <h5>{{doc.position}}</h5>
      <div>{{doc.description}}
      </div>
    </div>
</div>
{% endif %}
{% endfor %}

