---
title: "Applied AI Lab - Research"
layout: gridlay
excerpt: "Applied AI Lab -- Research Themes."
sitemap: false
permalink: /research/
---


# Research

Focusing on application of AI (Machine Learning) on different domains such as Communication and Networking, Computer Vison, Cyber-physical systems, our research aims to address fundamental problems of these areas as well as to develop practical methods that enable impactful applications. The current directions are listed as follows:

{% assign number_printed = 0 %}
{% for prli in site.data.researchthemes %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if prli.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ prli.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/researchpic/{{ prli.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ prli.description }}</p>
  <p><em>Members: {{ prli.members }}</em></p>
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
