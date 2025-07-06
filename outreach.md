---
layout: default
title: Outreach
permalink: /outreach/
---

<h1 id="community-activities">Community Activities</h1>

{% for vishubproject in site.vishubprojects %}

<p>
  {% if vishubproject.link %}
  <a href="{{vishubproject.link }}" style="font-size:1.2em; font-weight:bold;">{{ vishubproject.title }}</a>
  {% else %}
  <a href="{{vishubproject.url }}" style="font-size:1.2em; font-weight:bold;">{{ vishubproject.title }}</a>  
  {% endif %}
  {{ vishubproject.description | markdownify }}
</p>
{% endfor %}