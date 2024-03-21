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
<br />
<br />
  {% if item.hasthesis %}
    Thesis:
    {% if item.haslink %}
        <span class="cvthesis"> <a href="{{item.link}}" >{{ item.thesis }}</a> </span>
    {% else %}
        <span class="cvthesis"> {{ item.thesis }} </span>
    {% endif %}
    <div class="cvadvisor"> advised by {{item.advisor}}. </div>
  {% endif %}
</div>
{% endfor %}

