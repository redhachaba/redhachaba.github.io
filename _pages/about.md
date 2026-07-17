---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a Ph.D. candidate in economics at Paris Panthéon Assas University, under the supervision of [Prof. Victor Hiller](https://sites.google.com/site/victorhiller/) and [Prof. Paul Maarek](https://sites.google.com/site/paulmaarek2/).

My research examines how interactions between economic, demographic, and political forces shape institutional change.

I visited Brown University in Fall 2025 (hosted by [Prof. Stelios Michalopoulos](https://sites.google.com/site/steliosecon/research?authuser=0)) and the University of Cambridge in Fall 2024 (hosted by [Prof. Toke Aidt](https://www.econ.cam.ac.uk/people/academic/toke-aidt)).

In January 2027, I will join the Paris School of Economics as a postdoctoral researcher.

{% include base_path %}

<h2 id="publications">Publications</h2>
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
