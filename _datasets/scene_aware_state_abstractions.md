---
layout: dataset
title: "On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning - Dataset"
year: 2024
tags: [manipulation, planning, simulation, point-clouds, predicates, mobile-robotics]
eth_collection_url: "https://doi.org/10.3929/ethz-b-000634113"
paper: "\"On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning\""
doi: "10.3929/ethz-b-000634113"
---

This dataset accompanies the publication **On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning**. It provides paired demonstrations and perception features for two predicates:

- **on_clutter**: 20,000 training and 2,000 test samples
- **inside_drawer**: 20,000 training and 2,000 test samples

Each sample contains:

1. Demonstration data from the PyBullet simulator, including full physics state and scene object metadata.
2. Bounding-box features extracted as described in the paper.
3. Individual object point clouds for training point-cloud auto-encoders.
4. Scene-level point clouds containing all objects for scene encoding.
5. Encoded point clouds generated with multiple point-cloud encoders.

The accompanying code for handling and experimenting with the data is available at [https://github.com/ethz-asl/predicate_learning](https://github.com/ethz-asl/predicate_learning).

## Data Access

➡️ **ETH Research Collection / DOI landing page:** <https://doi.org/10.3929/ethz-b-000634113>

## Citation

Please cite the dataset as:

> **On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning**. Dataset available at <https://doi.org/10.3929/ethz-b-000634113>.
