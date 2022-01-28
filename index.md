The **VisHub is an interdisciplinary research lab and hub for teaching, collaboration, and outreach around data visualization** hosted by the [Institute for Design Informatics](https://www.designinformatics.org/) and the [School of Informatics](https://www.ed.ac.uk/informatics) at the [University of Edinburgh](https://www.ed.ac.uk). We research creative methods for interactive, exploratory and explanatory data visualizations across domains and environments (e.g., screen, physical, immersion). Our goal is to make data visualiztion and data analytics understandable by everyone. Find out more about our [research](#projects) and [outreach](#community-activities) below and don't hestitate to get in touch.

# News
- **Vistorian Updated Version launched *(Jan 2022)*:** The Vistorian network visualization platform comes with an new wizard making data upload easier. Visit the Vistorian and our training reseources on [http://vistorian.net](http://vistorian.net).
- **4 IEEE VIS papers (*October 2021*):** VisHub involved in 4 full papers and 2 workshops at [IEEE VIS 2021](http://ieeevis.org): [Workshop on VisActivities](https://visactivities.github.io) and Workshop on Visualization for Digital Humanities [VIS4DH](http://www.vis4dh.org/). Check the [VIS papers here](publications.html). 
- **Corona Moments Launched (*October 2021*):** We just launched a visualization as a retrospective on the pandemic. Please, help our research by exploring the interface and participating in the research: [corona memories](https://uclab.fh-potsdam.de/coronamemories) (In collaboration with the [Urban Complexity Lab](https://uclab.fh-potsdam.de/))
- **Uta Hinrichs joining as Reader (*September 2021*):** [Uta Hinrichs](http://www.utahinrichs.de) joins the VisHub as a Reader. Welcome Uta!!!
- **4 papers accepted to ACM CHI (*Dec 2020*):** Check our [publications](publications.html)!
<!--- **May 2021:** Starting the 2nd turn of our [Online Data Visualization Course for Professionals](https://datavis-online.github.io) on May 4th.
-  **April 2020:** >> **WE'RE HIRING** for 3(!) postdoc and engineer positions on [networks, storytelling and vis literacy](jobs-viscovery.html) as well as [vis in health](jobs-health.html).
-   **Dec 2020:** **Four full [papers](publications.html)** accepted at ACM CHI 2021!!
 -   _Oct 2020:_ [PhD Scholarship](phd-graphics-medicine.html) in Visualising Complex Care Pathways in Later Life.
-   _Oct 2020:_ Three full [papers](publications.html) accepted at [IEEE VIS 2020](http://ieeevis.org)!
-   _Oct 2020:_ Co-organizing [IEEE VIS Workshop on Guidelines in Visualiztion: VisGuides](https://nms.kcl.ac.uk/c4pgv).
-   _Oct 2020:_ Co-organizing [IEEE VIS Workshop on Visualization Education: VisActitivies](http://visactivities.github.io). -->
-   [..more](news.html)

[More news...](news.html)

<!-- to make the nav link work -->


<h1 id="projects">Research Topics & Projects</h1>

{% for project in site.projects %}
{% include projectpreview.html item=project %}
<!--   <h3><a href="{{project.url }}">{{ project.title }}</a></h3>
  <p>{{ project.description | markdownify }}</p> -->
{% endfor %}

<h1 id="community-activities">Community Activities</h1>

  <a href="https://groups.google.com/g/vishub-community" style="font-size:1.2em; font-weight:bold;">VisHub Community Mailing List</a>
  
 Join our mailing list focusing on data visualization in Edinburgh, Scotland, the UK and beyond. The group is open to everyone and aims to share news, events, discussions, jobs, etc.


{% for vishubproject in site.vishubprojects %}
  <p>
  {% if vishubproject.link %}
  <a href="{{vishubproject.link }}" style="font-size:1.2em; font-weight:bold;">{{ vishubproject.title }}</a>
  {% else %}
  <a href="{{vishubproject.url }}" style="font-size:1.2em; font-weight:bold;">{{ vishubproject.title }}</a>  
  {% endif %}
  {{ vishubproject.description | markdownify }}
</p>
<br/>
{% endfor %}
