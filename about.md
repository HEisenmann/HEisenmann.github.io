---
layout: single
author_profile: true
title: About me
toc: true
toc_sticky: true
---

{% assign publications = site.publications | sort: "year" | reverse %}

{% for pub in publications %}
{% if pub.title == 'A convergent adaptive finite element stochastic Galerkin method based on multilevel expansions of random fields' %}
    {%assign PubAdapt = pub %}
{% endif %}
{% if pub.title == 'Solving two-parameter eigenvalue problems using an alternating method' %}
    {%assign PubMEP = pub %}
{% endif %}
{% if pub.title == 'Existence of dynamical low-rank approximations to parabolic problems' %}
    {%assign PubDLR = pub %}
{% endif %}
{% if pub.title == 'Dynamical low-rank tensor approximations to high-dimensional parabolic problems: existence and convergence of spatial discretizations' %}
    {%assign PubDLR2 = pub %}
{% endif %}
{% if pub.title == 'Maximum relative distance between real rank-two and rank-one tensors' %}
    {%assign PubDistance = pub %}
{% endif %}

{% endfor %}

<figure>
<img src="/assets/pictures/meformal.jpg" style="width:300px;height:400px;">
</figure>

<div class="blocked">
Hello! I am Henrik Eisenmann, currently a postdoctoral researcher at IGPM RWTH Aachen. 
</div>

## Research interestes

<div class="blocked">
My current focus lies in adaptive algorithms for finding approximate solutions to partial differential equations. In my time at IGPM, I have already learned a lot about this topic. For a glimpse of our work, see my paper with Markus Bachmayr, Martin Eigel and Igor Voulis accessible <a style="color:0000A0"  href="{{PubAdapt.link}}"> here</a>.
</div>
<div class="blocked">
Since my master's thesis, I've been intrigues by eigenvalue problems. My master thesis was about solving eigenvalue problems in high dimensions utilizing special tensor formats. Subsequently, during my doctoral studies, I also learned about a generalization of eigenvalue problems with multiple eigenvalue parameters and equations.  A related piece of work with Yuji Nakatsukasa can be found <a style="color:0000A0" href="{{PubMEP.link}}"> here</a>.
</div>
<div class="blocked">
Furthermore, I'm deeply involved in exploring tensors, their multilinear aspects, and compressed low-rank tensor formats. Low-rank tensor formats are an interesting object to find and compress approximate solutions to PDEs. For parabolic equations, <a style="color:0000A0" href="{{PubDLR.link}}"> this work</a> with my Markus Bachmayr, Emil Kieri and André Uschmajew and <a style="color:0000A0" href="{{PubDLR2.link}}"> this collaboration</a> with Markus Bachmayr and André Uschmajew are noteworthy. They are concerned with the well-posedness of underlying infinite dimensional problems, whose solutions are approximated via actual numerical schemes. 
Another interesting projects concerns an abstract property of low-rank tensors. André Uschmajew and I computed the maximal distance a rank-two tensor can ever have from the set of rank-one tensors in <a style="color:0000A0" href="{{PubDistance.link}}"> this paper</a>.
</div>
## Personal

<div class="blocked">
I am currently active in the Handball club Schwarz-Rot Aachen. I am happy with the previous season, where we clinched the third position in the Kreisklassse 2 Aachen/Düren.
</div>
<div class="blocked">
Two years ago, I also started playing chess. It is a very captivating game, and fun for people at multiple levels of expertise.
</div>
