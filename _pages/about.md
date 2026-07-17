---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a PhD candidate in economics at Paris Panthéon Assas University, supervised by Victor Hiller and Paul Maarek.

My research examines how interactions between economic, demographic, and political forces shape institutional change.

I visited Brown University in Fall 2025 (hosted by Prof. Michalopoulos) and the University of Cambridge in Fall 2024 (hosted by Prof. Aidt).

In January 2027, I will join the Paris School of Economics as a postdoctoral researcher.

{% include base_path %}

## Publications
{% assign publications_list = site.publications | where: "category", "publication" | sort: "order" %}
{% for post in publications_list %}
  {% include archive-single.html %}
{% endfor %}

## Working Papers
{% assign workingpapers_list = site.publications | where: "category", "workingpaper" | sort: "order" %}
{% for post in workingpapers_list %}
  {% include archive-single.html %}
{% endfor %}

## Work in Progress
{% assign wip_list = site.publications | where: "category", "wip" | sort: "order" %}
{% for post in wip_list %}
  {% include archive-single.html %}
{% endfor %}
