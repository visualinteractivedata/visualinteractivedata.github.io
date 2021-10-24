The **VisHub is an interdisciplinary research lab and hub for teaching, collaboration, and outreach around data visualization** hosted by the [Institute for Design Informatics](https://www.designinformatics.org/) and the [School of Informatics](https://www.ed.ac.uk/informatics) at the [University of Edinburgh](https://www.ed.ac.uk). We research creative methods for interactive, exploratory and explanatory data visualizations across domains and environments (e.g., screen, physical, immersion). Our goal is to make data visualiztion and data analytics understandable by everyone. Find out more about our [research](#projects) and [outreach](#community-activities) below and don't hestitate to get in touch.

# News
- **October 2021:** VisHub involved in 4 :page_facing_up: full papers and 2 :speech_balloon: workshops at [IEEE VIS 2021](http://ieeevis.org): [Workshop on VisActivities](https://visactivities.github.io) and Workshop on Visualization for Digital Humanities [VIS4DH](http://www.vis4dh.org/). Check the [VIS papers here](publications.html). 
- **October 2021:** We just :loudspeaker: launched a :chart_with_upwards_trend: visualization as a retrospective on the pandemic. Please, help our :mag: research by exploring the interface and participating in the research: [corona memories](https://uclab.fh-potsdam.de/coronamemories) (In collaboration with the [Urban Complexity Lab](https://uclab.fh-potsdam.de/))
- **September 2021:** [Uta Hinrichs](http://www.utahinrichs.de) joins the VisHub as a Reader. Welcome Uta!!!
- **May 2021:** Starting the 2nd turn of our [Online Data Visualization Course for Professionals](https://datavis-online.github.io) on May 4th.
-  **April 2020:** >> **WE'RE HIRING** for 3(!) postdoc and engineer positions on [networks, storytelling and vis literacy](jobs-viscovery.html) as well as [vis in health](jobs-health.html).
-   **Dec 2020:** **Four full [papers](publications.html)** accepted at ACM CHI 2021!!
<!-- -   _Oct 2020:_ [PhD Scholarship](phd-graphics-medicine.html) in Visualising Complex Care Pathways in Later Life.
-   _Oct 2020:_ Three full [papers](publications.html) accepted at [IEEE VIS 2020](http://ieeevis.org)!
-   _Oct 2020:_ Co-organizing [IEEE VIS Workshop on Guidelines in Visualiztion: VisGuides](https://nms.kcl.ac.uk/c4pgv).
-   _Oct 2020:_ Co-organizing [IEEE VIS Workshop on Visualization Education: VisActitivies](http://visactivities.github.io). -->
-   [..more](news.html)

[More news...](news.html)

<!-- to make the nav link work -->
<h1 id="community-activities">Community Activities</h1>

{% for vishubproject in site.vishubprojects %}
  {% if vishubproject.link %}
  <h3><a href="{{vishubproject.link }}">{{ vishubproject.title }}</a></h3>
  {% else %}
  <h3><a href="{{vishubproject.url }}">{{ vishubproject.title }}</a></h3>  
  {% endif %}

  <p>{{ vishubproject.description | markdownify }}</p>
{% endfor %}


<h1 id="projects">Research Topics & Projects</h1>

{% for project in site.projects %}
{% include projectpreview.html item=project %}
<!--   <h3><a href="{{project.url }}">{{ project.title }}</a></h3>
  <p>{{ project.description | markdownify }}</p> -->
{% endfor %}
