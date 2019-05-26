---
layout: archive
permalink: /blog/
title: "Opinions"
author_profile: true
---

{% for cat in site.categories %}
  {% assign cat_name = cat[0] %}
  {% if cat_name == "blog" %}
    {% for post in site.categories[cat_name] %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
{% endfor %}
