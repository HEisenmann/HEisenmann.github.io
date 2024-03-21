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
    <span class="cvtime">{{ item.time }}</span> at <span class="cvinstitute"> {{item.institute}}.</span>
</div>
<div class="cvitem">
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

