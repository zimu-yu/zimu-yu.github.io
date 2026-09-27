---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
description: "Research projects by Zimu Yu in protein fitness landscapes, epistasis, and single-cell omics."
---

{% include base_path %}

{% assign projects = site.portfolio | sort: "order" %}
{% for post in projects %}
  {% include archive-single.html %}
{% endfor %}
