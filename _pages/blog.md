---
layout: archive
permalink: /blog/
title: "Blog Posts"
author_profile: true
classes: wide
---
----

>  "In God, we trust. All others must bring data."
>   W. Edwards Deming

----

{% for cat in site.categories %}
  {% assign cat_name = cat[0] %}
  {% if cat_name == "blog" %}
    {% for post in site.categories[cat_name] %}
      {% include archive-single.html %}
    {% endfor %}
  {% endif %}
{% endfor %}
