---
title: Portfolio
layout: default
tags: [PlanGrid, Research, Interviews]
---
<section class="mb4" markdown="block">
Currently—Design + Research<br>
{% include link.html content="@Jaza Energy" link="https://jazaenergy.com" %}

Previously—Design + Research<br>
{% include link.html content="@PlanGrid, an Autodesk Company" link="https://plangrid.com" %}

Studying—Systems Design Engineering<br>
{% include link.html content="@University of Waterloo" link="https://uwaterloo.ca" %}

Seeking—Summer 2020 design or research internships.<br>
Learning—to be a better storyteller.
</section>

<section markdown="0">
<h2>Projects</h2>
{% for item in site.projects %}
	{% include portfolio-card.html project=item %}
{% endfor %}
</section>

<a href="#" class="dn-ns bg-near-black pa3 white br2 no-underline dim">
	Back to top
</a>