---
title: "Phenikaa AI Lab - Publications"
layout: publications
excerpt: "Phenikaa AI Lab -- Publications."
sitemap: true
permalink: /publications/
---


# Publications
Jump to: [2021](#2021), [2020](#2020), [2019](#2019)
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
