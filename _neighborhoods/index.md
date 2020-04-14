---
layout: default
title: Neighborhoods
date: 2019-07-23 21:12
author: Klahanie
categories: []
---

{% for doc in site.neighborhoods %}
{% if doc.title != "Neighborhoods" %}
<div class="row mb-4">
  <img class="img-thumbnail col-md-2" src="{{site.url}}{{doc.thumbnail}}">
    <div class="col-md-10">
      <h4>
      <a href="{{doc.url}}">{{doc.title}}</a>
      </h4>
      <div>{{doc.description}}
      </div>
    </div>
</div>
{% endif %}
{% endfor %}