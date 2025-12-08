---
layout: dataset
title: "Scene-aware Generative State Abstractions Dataset"
year: 2024
tags: [manipulation, planning, simulation, point-clouds, predicates, mobile-robotics]
eth_collection_url: "https://doi.org/10.3929/ethz-b-000634113"
paper: "J. F\u00f6rster, J. J. Chung, L. Ott, R. Siegwart, \"On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning\", IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2024."
doi: "10.3929/ethz-b-000634113"
---

This dataset accompanies the publication **On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning** (IROS 2024). It provides paired demonstrations and perception features for two predicates:

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

Please cite the dataset and paper as:

> J. F\u00f6rster, J. J. Chung, L. Ott, R. Siegwart, **\"On Learning Scene-aware Generative State Abstractions for Task-level Mobile Manipulation Planning\"**, IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2024, pp. 13599\u201113606. DOI: <https://doi.org/10.3929/ethz-b-000634113>.
