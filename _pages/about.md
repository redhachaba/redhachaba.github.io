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

## Research

{% include base_path %}

{% assign ordered_publications = site.publications | sort: "order" %}

{% for post in ordered_publications %}
{% include archive-single.html %}
{% endfor %}