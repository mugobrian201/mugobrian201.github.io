---
title: "Data Science Projects"
permalink: /projects/
layout: collection
collection: projects
entries_layout: grid
classes: wide
---

## Real-World Predictive Modeling Portfolio

Each project demonstrates the complete data science workflow: problem definition, data cleaning, exploratory analysis, model building, validation, and actionable insights. All code available on [GitHub](https://github.com/mugobrian201/portfolio).

{% assign sorted_projects = site.projects | sort: 'importance' | reverse %}

{% for post in sorted_projects %}
  {% include archive-single.html %}
{% endfor %}
