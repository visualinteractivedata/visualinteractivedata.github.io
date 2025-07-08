<img src="/figures/banner.png" alt="Vishub group photo" style="width:100%; height:auto; margin-bottom: 0.5rem;">


The **VisHub is an interdisciplinary research lab and hub for teaching, collaboration, and outreach around data visualization** hosted by the [Institute for Design Informatics](https://www.designinformatics.org/) and the [School of Informatics](https://www.ed.ac.uk/informatics) at the [University of Edinburgh](https://www.ed.ac.uk). We research creative methods for interactive, exploratory and explanatory data visualizations across domains and environments. Our goal is to make data visualization and data analytics understandable by everyone.

# News

{% assign newsList = site.pages | where:"name","news.md" | first %}
{{ newsList.excerpt }}

[More news...]({% link news.md %})

<h1 id="project">Projects</h1>

{% for project in site.project %}
{% include projectpreview.html item=project %}
{% endfor %}

<!-- <h1 id="projects">Research Topics</h1> -->

<!-- {% for r in site.research %}
  {% include projectpreview.html item=r %}
{% endfor %} -->

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
