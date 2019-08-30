---
layout: default
title: About
---
## About
<div class="mw6 mb4 lh-copy" markdown="block">
I’ve read a lot of student portfolio blurbs. They often consist of “why you design”, parts of ther design process you’re drawn to, and your hobbies to show that you have a life outside of work.

When I write this for real, I want to tell a story of where I come from, struggles I’ve faced to get to where I am now, and where I want to go. Perhaps like a journal entry.

![Beautiful asian man wearing a Canada hat, glasses and a blue shirt. Looking to the right.](/assets/images/me.jpg)
{: .mt3}
</div>



## Contact
<ul class="list pl0">
	{% for item in site.data.contact %}
		<li class="mb2"
		>{{ item.name }}: {% include link.html link=item.link content=item.handle %}</li>
	{% endfor %}
		<li>Resume: {% include link.html content="Download"%} | {% include link.html content="View online"%}</li>
</ul>