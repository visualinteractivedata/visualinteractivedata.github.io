---
layout: default
title: Projects
permalink: /projects/
---

<h1 id="projects">Projects</h1>

{%- assign all_tags = "" -%}
{%- for p in site.project -%}
  {%- if p.tags -%}
    {%- for t in p.tags -%}
      {%- assign all_tags = all_tags | append: t | append: "," -%}
    {%- endfor -%}
  {%- endif -%}
{%- endfor -%}
{%- assign all_tags = all_tags | split: "," | uniq | sort -%}

<ul class="menu tag-menu">
  <li><a class="tag-filter active" data-tag="all" href="#">All</a></li>
  {%- for tag in all_tags -%}
    {%- if tag != "" -%}
      <li><a class="tag-filter" data-tag="{{ tag | downcase }}" href="#">{{ tag }}</a></li>
    {%- endif -%}
  {%- endfor -%}
</ul>

<div id="project-list" class="project-grid">
{% assign sorted_projects = site.project | sort: "date" | reverse %}
{% for project in sorted_projects %}
  {% include projecttile.html item=project %}
{% endfor %}
</div>

<!-- <div id="project-list">
{% for project in site.project %}
  {% include projectpreview.html item=project %}
{% endfor %}
</div> -->

<script>
(function () {
  const buttons = document.querySelectorAll(".tag-filter");
  const cards = document.querySelectorAll(".project-tile");

  buttons.forEach((btn) => {
    btn.addEventListener("click", (e) => {
      e.preventDefault();
      buttons.forEach((b) => b.classList.remove("active"));
      btn.classList.add("active");
      const tag = btn.dataset.tag;
      cards.forEach((card) => {
        const tags = card.dataset.tags ? card.dataset.tags.split(",") : [];
        const match = tag === "all" || tags.includes(tag);
        card.style.display = match ? "" : "none";
      });
    });
  });
})();
</script>
