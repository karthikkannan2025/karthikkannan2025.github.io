---
layout: page
title: Projects
permalink: /Projects/
description: Personal builds, aircraft projects, and research — the decisions and lessons behind the work
nav: true
nav_order: 3
display_categories:
  - fun
  - research
---

I use projects to learn by building: start with an idea, work through the constraints, and find out what survives testing. Some of these are aircraft I helped build and fly; others are software projects or early concepts I am still working through.

[Personal builds](#fun) · [Aerospace & research](#research) · [Professional work]({{ '/experience/' | relative_url }})

<div class="projects">
{% for category in page.display_categories %}
  <h2 id="{{ category }}" class="category">{% if category == "fun" %}Personal Builds{% else %}Aerospace & Research{% endif %}</h2>
  {% assign sorted_projects = site.projects | where: "category", category | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
  {% for project in sorted_projects %}
    {% unless project.published == false %}
      {% include projects.liquid %}
    {% endunless %}
  {% endfor %}
  </div>
{% endfor %}
</div>
