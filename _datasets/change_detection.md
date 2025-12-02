---
layout: dataset
title: "Change Detection Datasets"
year: 2017
tags: [indoor, change-detection, TSDF, dynamic-objects]
eth_collection_url: "https://doi.org/10.3929/ethz-b-000721640"
paper: "M. Fehr, F. Furrer, I. Dryanovski, J. Sturm, I. Gilitschenski, R. Siegwart, C. Cadena, “TSDF-based change detection for consistent long-term dense reconstruction and dynamic object discovery”, IEEE ICRA 2017, pp. 5237-5244."
doi: "10.3929/ethz-b-000721640"
---

![Lounge environment snapshot](/assets/datasets/change-detection/teaser_sheeped.png)

This dataset suite presents three indoor change-detection scenarios collected by the Autonomous Systems Lab (ASL) at ETH Zurich. The corresponding publication is linked above.

## Dataset Description

The dataset contains **three indoor environments**:
- **office** – A controlled office scene with four tripod static observations.
- **lounge** – A challenging meeting-area/office lounge, hand-held recordings over two weeks, frequent object changes, varying overlap ~50–100%.
- **living_room** – A baseline scene with nine hand-held recordings in a controlled indoor environment, high overlap and multiple viewpoints.

Each scenario provides sequences of RGB-D (and potentially point cloud) data, dense reconstructions, and change annotations for use in benchmarking change-detection and dynamic-object-discovery algorithms.

## Data Access

- [ETH Research Collection Link](https://doi.org/10.3929/ethz-b-000721640)
- GitHub mirror / supplementary code: [ethz-asl/change_detection_ds](https://github.com/ethz-asl/change_detection_ds)

## Use Cases & Applications

- Long-term dense reconstruction and dynamic object discovery in indoor settings
- Benchmarking algorithms for change detection, TSDF-based scene modelling, dynamic scene segmentation
- Comparison of static vs. dynamic-object behaviour in indoor robotics environments

## Citation

> M. Fehr, F. Furrer, I. Dryanovski, J. Sturm, I. Gilitschenski, R. Siegwart, C. Cadena,
> **“TSDF-based change detection for consistent long-term dense reconstruction and dynamic object discovery.”**,
> IEEE International Conference on Robotics and Automation (ICRA) 2017, pp. 5237-5244.
> DOI: 10.3929/ethz-b-000721640

