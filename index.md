---
title: Portfolio
layout: default
---
<section class="f1-l f2-m f3 lh-title vh-75"
	style='min-height: calc(0.75 * 640px)'>
	<div>
		Hi, I’m Kevin Chan.<br><br>
		I like to think in systems,<br class='dn di-l'>
		tell stories about real people,<br class='dn di-l'>
		and help teams make decisions with research. <br><br>
		<a href='#projects'>See it in action. ↓</a>
	</div>
</section>

<section markdown="0" id='projects' class='pt5'>
{% for item in site.projects %}
	{% include portfolio-item.html project=item %}
{% endfor %}
</section>