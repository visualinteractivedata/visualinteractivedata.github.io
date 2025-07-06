---
layout: default
title: Projects
permalink: /project/
---

<h1 id="projects">Projects</h1>

{% for project in site.project %}
  {% include projectpreview.html item=project %}
{% endfor %}
