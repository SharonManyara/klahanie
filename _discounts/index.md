---
layout: default
title: Discounts
date: 2020-01-25 23:49
author: Klahanie
comments: true
categories: []
show-title: false
---

<img src="{{site.url}}/images/discounts/banner.jpg" class="img-fluid">

As a member of the HOA, this portion of the web site is dedicated to providing you with information about the companies we have selected to provide you with discounts on their services because you are an HOA member is good standing.

Each vendor has their own page to educate you about their products and services and the incentives they will provide to you when you use their products/ services. To make it easy for you to receive the benefits, each company will have a discount code on their page. Use this code when dealing with the company to insure that you receive the HOA Benefit you deserve.

Before you make any purchases for your home or garden, check back to this site to see the vendors added to this program.

{% for doc in site.discounts %}
{% if doc.title != "Discounts" %}

<div class="row mb-4">
  <img class="img-thumbnail col-md-2" src="{{site.url}}/{{doc.thumbnail}}">
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
