---
title: "Phenikaa AI Lab - Research"
layout: gridlay
excerpt: "Phenikaa AI Lab -- Research Themes."
sitemap: false
permalink: /courses/
---


# Training Courses

{% assign number_printed = 0 %}
{% for prli in site.data.courses %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if prli.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ prli.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/coursepic/{{ prli.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ prli.description }}</p>
  <p><em>Lecturers: {{ prli.teachers }}</em></p>
  {% if prli.certificate %}
  <p> <em> {{ prli.certificate }} </em> </p>
  {% endif %}
  {% if prli.link.url %}
  <p><strong><a href="{{ prli.link.url }}">{{ prli.link.display }}</a></strong></p>
  {% endif %}
  {% if prli.new1 %}
  <p class="text-danger"><strong> {{ prli.news1 }}</strong></p>
  {% endif %}
  {% if prli.award %}
  <p> <em> {{ prli.award }} </em> </p>
  {% endif %}
  {% if prli.news2 %}
  <p> {{ prli.news2 }} </p>
  {% endif %}
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>
