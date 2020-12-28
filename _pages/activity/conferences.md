---
layout: page
---
<h2> Conferences (selection) </h2>
<div class="post">
<ul>
{% for c in site.data.conferenze %}
{% if c.attribute == "m" %}
	{% else %}
	<li> {{ c.title }}<br>
	{% if c.link %} 
	<a href="{{ c.link }}">
	{% endif %}
	{{ c.workshop }}
	{% if c.link %}
		</a>
		{% endif %}<br>
		{{ c.location }}, {{ c.year }}
		</li>
	{% endif %}
{% endfor %}
</ul>

</div>
