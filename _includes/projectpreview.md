<div class="pubWrapper">
	<div class="pubImage">
		<img src="{{ include.item.image }}"/>
	</div>

	<div class="pubText">
		<p>
			<a href="{{ include.item.url }}"
        		style="font-weight: bold;"
			target="_blank"
			>{{ include.item.title }}</a> 
        		{{ include.item.description | markdownify }}
		</p>
	</div>
</div>
