---
layout: archive
permalink: /signal-processing/
title: "Signal Processing Projects"
author_profile: true
#header:
#  image: "/images/security-camera.jpg"
#  caption: "Photo credit: [**Pexels**](https://www.pexels.com)"
---

{% for cat in site.categories %}
  {% assign cat_name = cat[0] %}
  {% if cat_name == "signal" %}
    {% for post in site.categories[cat_name] %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
{% endfor %}
