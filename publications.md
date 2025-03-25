---
layout: single
author_profile: true
title: Publications
toc: true
toc_label: published in
toc_sticky: true
---

{% assign publications = site.publications | sort: "year" | reverse %}

## 2025

{% for pub in publications %}
{% if {{pub.year}} == 2025 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }}</div>
  <div class="pubinfo"><a href="{{pub.doilink}}" >{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</a></div>
</div>
{% endif %}
{% endfor %}

## 2024

{% for pub in publications %}
{% if {{pub.year}} == 2024 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }}</div>
  <div class="pubinfo"><a href="{{pub.doilink}}" >{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</a></div>
</div>
{% endif %}
{% endfor %}

## 2023

{% for pub in publications %}
{% if {{pub.year}} == 2023 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }}</div>
    <div class="pubinfo"><a href="{{pub.doilink}}" >{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</a></div>
</div>
{% endif %}
{% endfor %}


## 2022

{% for pub in publications %}
{% if {{pub.year}} == 2022 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.link}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }}</div>
  <div class="pubinfo"><a href="{{pub.doilink}}" >{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</a></div>
  </div>
{% endif %}
{% endfor %}


## 2021

{% for pub in publications %}
{% if {{pub.year}} == 2021 %}
<div class="pubitem">
  <div class="pubtitle"><a href="{{pub.arxivlink}}" >{{ pub.title }}</a> </div>
  <div class="pubauthors">{{ pub.authors }}</div>
  <div class="pubinfo"><a href="{{pub.doilink}}" >{{ pub.journal }} {{pub.volume}}, {{ pub.year}}.</a></div>
</div>
{% endif %}
{% endfor %}

