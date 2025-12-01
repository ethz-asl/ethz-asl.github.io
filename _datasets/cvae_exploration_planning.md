---
layout: dataset
title: "CVAE Exploration Planning Data"
year: 2022
tags: [exploration, planning, learning, mapping]
eth_collection_url: ""
paper: "L. Schmid, C. Ni, et al., “Fast and Compute-efficient Sampling-based Local Exploration Planning via Distribution Learning”, IEEE Robotics and Automation Letters (RA-L), 2022."
doi: ""
---

Data accompanying the CVAE exploration planning project, providing local maps with supervision signals for conditional variational autoencoder and CNN models used in learning-based exploration.

Repository: [cvae_exploration_planning](https://github.com/ethz-asl/cvae_exploration_planning) • Preprint on [ArXiv](https://arxiv.org/abs/2202.13715)

## Data Layout

- `CVAE_dataset.npy`: Local maps with best actions from a teacher planner (supervision for CVAE)
- `CNN_dataset.npy`: Local maps with random actions (CNN training set)
- `test_worlds.zip`: Test worlds
  - `<environment>_<no>.p`: Pickled test world
  - `<environment>_<no>.txt`: Initial pose `[x, y, yaw]`

Additional utilities for processing and ROS playback are in the [panoptic_mapping](https://github.com/ethz-asl/panoptic_mapping) repository.

## Downloads

- Dataset landing page: **Research Collection link pending** (was `2022_CVAE_Exploration_Planning/`)
- CVAE dataset (326.4 MB): **Research Collection link pending** (was `CVAE_dataset.npy`)
- CNN dataset (1.0 GB): **Research Collection link pending** (was `CNN_dataset.npy`)
- Test worlds (56.5 KB): **Research Collection link pending** (was `test_worlds.zip`)

## Citation

> L. Schmid, C. Ni, et al.,  
> **“Fast and Compute-efficient Sampling-based Local Exploration Planning via Distribution Learning”**, IEEE Robotics and Automation Letters (RA-L), 2022.
