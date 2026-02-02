---
layout: default
title: Research
permalink: /research/
---

<h1 id="projects">Research Topics & Projects</h1>

{% for r in site.research %}
  {% include projectpreview.html item=r %}
{% endfor %}
