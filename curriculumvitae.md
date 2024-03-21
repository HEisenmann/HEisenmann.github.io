---
layout: single
author_profile: true
title: Curriculum Vitae
usemathjax: true
toc: true
toc_sticky: true
---

{% assign cv = site.cvitems | sort: "year" | reverse %}

{% for item in cv %}

## {{ item.title }} 

<div class="cvitem">
  <div class="cvtime">{{ item.time }} at {{item.institute}}.</div>
  {% if item.hasthesis %}
    {% if item.haslink %}
        <div class="cvthesis">Thesis: <a href="{{item.link}}" >{{ item.thesis }}</a> </div>
    {% else %}
        <div class="cvthesis">Thesis: {{ item.thesis }} </div>
    {% endif %}
    <div class="cvadvisor"> advised by {{item.advisor}}. </div>
  {% endif %}
</div>
{% endfor %}

