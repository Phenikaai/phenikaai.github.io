---
title: "Applied AI Lab - Projects"
layout: gridlay
excerpt: "Applied AI Lab -- Projects."
sitemap: false
permalink: /projects/
---


# Projects

{% assign number_printed = 0 %}
{% for prli in site.data.projectlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if prli.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ prli.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pjpic/{{ prli.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ prli.description }}</p>
  <p><em>Members: {{ prli.members }}</em></p>
  <p><strong><a href="{{ prli.link.url }}">{{ prli.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ prli.news1 }}</strong></p>
  <p> <em> {{ prli.award }} </em> </p>
  <p> {{ prli.news2 }} </p>
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
