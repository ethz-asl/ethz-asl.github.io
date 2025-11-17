---
layout: dataset
title: "ASL Datasets"
permalink: /datasets/
---

<p>
This page lists datasets recorded at the Autonomous Systems Lab.
The actual data files are hosted on the ETH Research Collection and other long-term repositories.
</p>

<ul>
{% assign sorted = site.datasets | sort: "year" | reverse %}
{% for ds in sorted %}
  <li>
    <a href="{{ ds.url }}">{{ ds.title }}</a>
    {% if ds.year %} ({{ ds.year }}){% endif %}
  </li>
{% endfor %}
</ul>