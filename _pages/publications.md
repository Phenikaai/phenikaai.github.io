---
title: "Phenikaa AI Lab - Publications"
layout: publications
excerpt: "Phenikaa AI Lab -- Publications."
sitemap: true
permalink: /publications/
---


# Publications
Jump to: [2022](#2022),[2021](#2021), [2020](#2020), [2019](#2019)
## 2022
{% assign order = 1 %}
{% for publi in site.data.pub.2022 %}
  {% increment order %}
  <p style="color: black">
  {order}. {{ publi.authors }}, "<a href="{{ publi.link.url }}">{{ publi.title }}</a>," {{ publi.link.display }}
  </p>
{% endfor %}

## 2021
{% assign order = 1 %}
{% for publi in site.data.pub.2021 %}
  {% increment order %}
  <p style="color: black">
  {order}. {{ publi.authors }}, "<a href="{{ publi.link.url }}">{{ publi.title }}</a>," {{ publi.link.display }}
  </p>
{% endfor %}

## 2020
{% assign order = 1 %}
{% for publi in site.data.pub.2020 %}
  <p style="color: black">
  {% increment order %}. {{ publi.authors }}, "<a href="{{ publi.link.url }}">{{ publi.title }}</a>," {{ publi.link.display }}
  </p>
{% endfor %}

## 2019
{% for publi in site.data.pub.2019 %}

  {{ publi.title }} ,
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}"><b>{{ publi.link.display }}</b></a>

{% endfor %}
