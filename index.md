---
title: Portfolio
layout: default
tags: [PlanGrid, Research, Interviews]
---
<section class="mb4 lh-copy mt0" markdown="block">
Seeking—Summer 2020 design or research internships.<br>
Learning—to be a better storyteller.
</section>

<section markdown="0">
<!-- <h2>Projects</h2> -->
{% for item in site.projects %}
	{% include portfolio-card.html project=item %}
{% endfor %}
</section>

<a href="#" class="dn-ns bg-near-black pa3 white br2 no-underline dim">
	Back to top
</a>