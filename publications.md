---
layout: single
author_profile: true
title: Publications
toc: true
---

{% assign publications = site.publications | sort: "year" | reverse %}

## 2024

{% for pub in publications %}
{% if {{pub.year}} == 2024 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }};</div>
  <div class="pubinfo">{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</div>
</div>
{% endif %}
{% endfor %}

## 2023

{% for pub in publications %}
{% if {{pub.year}} == 2023 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }};</div>
  <div class="pubinfo">{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</div>
</div>
{% endif %}
{% endfor %}


## 2022

{% for pub in publications %}
{% if {{pub.year}} == 2022 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }};</div>
  <div class="pubinfo">{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</div>
</div>
{% endif %}
{% endfor %}


## 2021

{% for pub in publications %}
{% if {{pub.year}} == 2021 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }};</div>
  <div class="pubinfo">{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</div>
</div>
{% endif %}
{% endfor %}

