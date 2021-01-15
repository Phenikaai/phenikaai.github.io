---
title: "Applied AI Lab - Publications"
layout: publications
excerpt: "Applied AI Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## 2021
{% for publi in site.data.pub.2021 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

## 2020
{% for publi in site.data.pub.2020 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

## 2019
{% for publi in site.data.pub.2019 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
