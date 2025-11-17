---
layout: default
title: "ASL Datasets"
---

# ASL Datasets

This site lists datasets recorded by the [Autonomous Systems Lab](https://www.asl.ethz.ch) for the robotics community.
The actual data is hosted on the ETH Research Collection and other long-term storage systems.

{% assign sorted = site.datasets | sort: "year" | reverse %}
{% for ds in sorted %}
## [{{ ds.title }}]({{ ds.url }})

- **Year:** {{ ds.year }}
{% if ds.paper %}- **Paper:** {{ ds.paper }}{% endif %}
{% if ds.eth_collection_url %}- **Data:** [ETH Research Collection]({{ ds.eth_collection_url }}){% endif %}
{% if ds.tags %}- **Tags:** {{ ds.tags | join: ", " }}{% endif %}

{% endfor %}