---
layout: default
title: Contact
---
<section>
<ul class="list pl0">
	{% for item in site.data.contact %}
		<li class="mb2"
		>{{ item.name }}: {% include link.html link=item.link content=item.handle %}</li>
	{% endfor %}
		<li>Resume: {% include link.html content="Download"%} | {% include link.html content="View online"%}</li>
</ul>
</section>