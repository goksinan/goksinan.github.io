---
layout: archive
permalink: /machine-learning/
title: "Machine Learning Projects"
author_profile: true
#header:
#  image: "/images/artificial-intelligence.jpg"
#  caption: "Photo credit: [**Starline**](https://www.freepik.com/free-vector/cyber-technology-concept-design_2393316.htm)"
---

{% for cat in site.categories %}
  {% assign cat_name = cat[0] %}
  {% if cat_name == "machine" %}
    {% for post in site.categories[cat_name] %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
{% endfor %}
