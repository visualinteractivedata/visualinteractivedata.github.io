<div class="pubWrapper">
	<div class="pubImage">
		<img src="{{ include.item.image }}"/>
	</div>

	<div class="pubText">
		<p>
			<a
        {% if vishubproject.link %}
				href="{{ include.item.link }}"
				{% else %}
				href="{{ include.item.url }}"
        {% endif %}
        style="font-weight: bold;"
				target="_blank"
				> {{ include.item.title }}</a> 
        {{ vishubproject.description | markdownify }}
		</p>
	</div>
</div>
