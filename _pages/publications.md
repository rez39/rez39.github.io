---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
---


  You can also find my articles on my [Google Scholar](https://scholar.google.com/citations?user=68eqQUsAAAAJ&hl=en)


{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
