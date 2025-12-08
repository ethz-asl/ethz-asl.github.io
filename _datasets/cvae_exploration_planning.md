---
layout: dataset
title: "CVAE Exploration Planning Data"
year: 2022
tags: [exploration, planning, learning, mapping]
eth_collection_url: "https://doi.org/10.3929/ethz-c-000788332"
paper: "L. Schmid, C. Ni, et al., “Fast and Compute-efficient Sampling-based Local Exploration Planning via Distribution Learning”, IEEE Robotics and Automation Letters (RA-L), 2022."
doi: "10.3929/ethz-c-000788332"
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

- Dataset landing page: <https://doi.org/10.3929/ethz-c-000788332>
- CVAE dataset (326.4 MB): <https://doi.org/10.3929/ethz-c-000788332>
- CNN dataset (1.0 GB): <https://doi.org/10.3929/ethz-c-000788332>
- Test worlds (56.5 KB): <https://doi.org/10.3929/ethz-c-000788332>

## Citation

> L. Schmid, C. Ni, et al.,  
> **“Fast and Compute-efficient Sampling-based Local Exploration Planning via Distribution Learning”**, IEEE Robotics and Automation Letters (RA-L), 2022.
