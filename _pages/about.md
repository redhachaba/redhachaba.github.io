---
permalink: /
title: "Redha Chaba"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome! I'm a PhD candidate in economics at Paris Panthéon Assas University, supervised by Victor Hiller and Paul Maarek. My research examines how interactions between economic, demographic, and political forces shape institutional change.
I visited Brown University in Fall 2025 (hosted by Prof. Michalopoulos) and the University of Cambridge in Fall 2024 (hosted by Prof. Aidt). In January 2027, I will join the Paris School of Economics as a postdoctoral researcher.

## Research

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h3>{{ category[1].title }}</h3><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}