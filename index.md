---
title: Portfolio
layout: default
tags: [PlanGrid, Research, Interviews]
---
<section class="f1-l f2-m f3 lh-title vh-75" markdown="block">
Hi, I’m Kevin Chan.

I like to think in systems,<br>
tell stories about real people,<br>
and help teams make decisions with research.

See it in action. ↓
</section>
<!-- <a href='/'>test</a> -->

<section markdown="0">
<!-- <h2>Projects</h2> -->
{% for item in site.projects %}
	{% include portfolio-item.html project=item %}
{% endfor %}
</section>