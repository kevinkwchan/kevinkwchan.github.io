---
title: Portfolio
layout: default
tags: [PlanGrid, Research, Interviews]
---
<section class="f1-l f2-m f3 lh-title vh-75"
	style='min-height: calc(0.75 * 640px)'>
	<div>
		Hi, I’m Kevin Chan.<br><br>
		I like to think in <span class='bg-yellow'>systems</span>,<br class='dn di-l'>
		tell <span class='bg-yellow'>stories</span> about real people,<br class='dn di-l'>
		and help teams make decisions with <span class='bg-yellow'>research</span>. <br><br>
		See it in action. ↓
		<!-- <a href='#projects'>See it in action. ↓</a> -->
	</div>
</section>

<section markdown="0" id='projects' class=''>
{% for item in site.projects %}
	{% include portfolio-item.html project=item %}
{% endfor %}
</section>