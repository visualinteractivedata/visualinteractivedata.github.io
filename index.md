The **VisHub** is an interdisciplinary research lab researching creative methods for interactive, exploratory and explanatory data visualizations across domains and environments (e.g., screen, physical, immersion). Our goal is to make data visualiztion and data analytics understandable by everyone. We are based at the [Institute for Design Informatics](https://www.designinformatics.org/) and the [School of Informatics](https://www.ed.ac.uk/informatics) at the [University of Edinburgh](https://www.ed.ac.uk). Our research includes, but is not limited to:

-   data-driven storytelling,
-   visualization education
-   immersive Analytics,
-   network and spatio-temporal visualization,
-   physical visualization,
-   data visualization and NLP

We are heavily involved in co-organizing [Edinburgh's Data Vis Meetup](https://www.meetup.com/meetup-group-vBHbCmgh). [Get in touch with us](mailto:bbach@ed.ac.uk) if you want to become involved. Likewise, every last Friday of the month, we're running a [Chart Clinic](chart-clinic.html) for staff and graduat(e/ing) studnets of the University.

# News
- _September 2021:_ [Uta Hinrichs](http://www.utahinrichs.de) is joins the VisHub as a Reader. Welcome Uta!!!
- _May 2021:_ Starting the 2nd turn of our [Online Data Visualization Course for Professionals](https://datavis-online.github.io) on May 4th.
-  _April 2020:_ >> **WE'RE HIRING** for 3(!) postdoc and engineer positions on [networks, storytelling and vis literacy](jobs-viscovery.html) as well as [vis in health](jobs-health.html).
-   _Dec 2020:_ **Four full [papers](publications.html)** accepted at ACM CHI 2021!!
-   _Oct 2020:_ [PhD Scholarship](phd-graphics-medicine.html) in Visualising Complex Care Pathways in Later Life.
-   _Oct 2020:_ Three full [papers](publications.html) accepted at [IEEE VIS 2020](http://ieeevis.org)!
-   _Oct 2020:_ Co-organizing [IEEE VIS Workshop on Guidelines in Visualiztion: VisGuides](https://nms.kcl.ac.uk/c4pgv).
-   _Oct 2020:_ Co-organizing [IEEE VIS Workshop on Visualization Education: VisActitivies](http://visactivities.github.io).
-   [..more](news.html)

[More news...](news.html)

<!-- to make the nav link work -->

<h1 id="projects">Outreach Activities</h1>

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
  <h3><a href="{{project.url }}">{{ project.title }}</a></h3>

<!--   {% if project.image %}
  <a href="{{project.url }}"><img src="{{project.image}}" /></a>
  {% endif %}
 -->
  <p>{{ project.description | markdownify }}</p>
{% endfor %}
