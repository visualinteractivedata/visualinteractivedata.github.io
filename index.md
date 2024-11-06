The **VisHub is an interdisciplinary research lab and hub for teaching, collaboration, and outreach around data visualization** hosted by the [Institute for Design Informatics](https://www.designinformatics.org/) and the [School of Informatics](https://www.ed.ac.uk/informatics) at the [University of Edinburgh](https://www.ed.ac.uk). We research creative methods for interactive, exploratory and explanatory data visualizations across domains and environments (e.g., screen, physical, immersion). Our goal is to make data visualization and data analytics understandable by everyone. Find out more about our [research](#projects) and [outreach](#community-activities) below and don't hesitate to get in touch.

# News

- Hiring a [visualization designer / workshop facilitator](jobs/co-benefits-atlas) for a project on building a UK-wide Co2 emission-reduction Co-Benefits atlas. Starting now untli July 2025.
- Weloming [Dorkey Kaufmann](https://www.linkedin.com/in/dorseykaufmann) in our group!
- [4 full papers and 1 VISAPP paper](publications.html) accepted to IEEE VIS.
- ~~Hiring for a [visualization researcher / designer / developer](jobs/visres2024) for March-June 2024.~~
- ~~Hiring for a [permanent teaching position](https://elxw.fa.em3.oraclecloud.com/hcmUI/CandidateExperience/en/sites/CX_1001/job/8990) at the intersection of data, design and technology.~~
- We are hosting the international [Information+ conference](https://informationplusconference.com/) on information design and data visualization in Edinburgh in November 2023.
- [Join us for a **PhD** and check our topics](jobs/index.html)
- [Lara Johnson and Rea Michalopoulou](people.html) joining us as PhD students.
- **3 [Full papers](publications.html) accepted for [IEEE VIS 2022](http://ieeevis.org/year/2022/welcome)**, two of which have won **honorable mention**s!!
- **Vistorian Updated Version launched _(Jan 2022)_:** The Vistorian network visualization platform comes with an new wizard making data upload easier. Visit the Vistorian and our training resources on [http://vistorian.net](http://vistorian.net).
- **2 [full papers](publications.html) accepted for [ACM CHI 2022](https://chi2022.acm.org)!!**
- **Open PhD positions (_Dec 2021_):** Check at [Positions/PhD](https://visactivities.github.io/jobs) and get in touch with Uta Hinrichs and Ben Bach.
- **4 IEEE VIS papers (_Oct 2021_):** VisHub involved in 4 full papers and 2 workshops at [IEEE VIS 2021](http://ieeevis.org): [Workshop on VisActivities](https://visactivities.github.io) and Workshop on Visualization for Digital Humanities [VIS4DH](http://www.vis4dh.org/). Check the [VIS papers here](publications.html).
- **Corona Moments Launched (_October 2021_):** We just launched a visualization as a retrospective on the pandemic. Please, help our research by exploring the interface and participating in the research: [corona memories](https://uclab.fh-potsdam.de/coronamemories) (In collaboration with the [Urban Complexity Lab](https://uclab.fh-potsdam.de/))
- **Uta Hinrichs joining as Reader (_September 2021_):** [Uta Hinrichs](http://www.utahinrichs.de) joins the VisHub as a Reader. Welcome Uta!!!

[More news...](news.html)

<!-- to make the nav link work -->

<h1 id="projects">Research Topics & Projects</h1>

{% for project in site.projects %}
{% include projectpreview.html item=project %}

<!--   <h3><a href="{{project.url }}">{{ project.title }}</a></h3>
  <p>{{ project.description | markdownify }}</p> -->

{% endfor %}

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
