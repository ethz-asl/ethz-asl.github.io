---
layout: dataset
title: "Panoptic Multi-TSDFs Data"
year: 2022
tags: [panoptic, mapping, tsdf, synthetic, indoor]
eth_collection_url: ""
paper: "L. Schmid et al., “Panoptic Multi-TSDFs: a Flexible Representation for Online Multi-resolution Volumetric Mapping and Long-term Dynamic Scene Consistency”, IEEE International Conference on Robotics and Automation (ICRA), 2022."
doi: ""
---

Datasets for the Panoptic Multi-TSDFs project, including a synthetic indoor “flat” dataset rendered in Unreal Engine and supplementary panoptic data for RIO sequences to run the panoptic mapping pipeline.

Code: [panoptic_mapping](https://github.com/ethz-asl/panoptic_mapping) • Papers: [IEEE](https://ieeexplore.ieee.org/abstract/document/9811877) | [ArXiv](https://arxiv.org/abs/2109.10165)

![Panoptic mapping flat dataset runs](/assets/datasets/panoptic_mapping/panoptic_mapping_run1.png)
![Panoptic mapping flat dataset run 2](/assets/datasets/panoptic_mapping/panoptic_mapping_run2.png)
![Panoptic mapping changes overview](/assets/datasets/panoptic_mapping/panoptic_mapping_changes.png)

## Flat Dataset

- Two trajectories in a changing indoor environment with panoptic annotations
- Per frame: color PNG, depth TIFF (m), panoptic GT labels, Detectron2 predictions and metadata, pose, timestamps
- Ground-truth structure: `flat_<RunNo>_gt_10000.ply`
- Utility files: label maps, detectron labels, change log, intrinsics
- Simulator configuration (airsim.yaml), corrections, and waypoint logs included

## RIO Demo Data

- Additional panoptic labels and point clouds for RIO scan IDs:
  `0cac7578-8d6f-2d13-8c2d-bfa7a04f8af3`,
  `20c9939d-698f-29c5-85c6-3c618e00061f`,
  `2451c041-fae8-24f6-9213-b8b6af8d86c1`,
  `ddc73793-765b-241a-9ecd-b0cebb7cf916`,
  `ddc73795-765b-241a-9c5d-b97744afe077`,
  `f62fd5f8-9a3f-2f44-8b1e-1289a3a61e26`
- Per sequence: panoptic labels (GT and Detectron2), per-sequence ground-truth point clouds, combined scene point clouds, label maps
- Original RIO data must be downloaded separately: [RIO dataset](https://waldjohannau.github.io/RIO/)

## Downloads

- Flat dataset (392.7 MB): **Research Collection link pending** (was `flat_dataset.zip`)
- RIO panoptic add-ons (87.8 MB): **Research Collection link pending** (was `rio_data.zip`)

## Citation

> L. Schmid et al.,  
> **“Panoptic Multi-TSDFs: a Flexible Representation for Online Multi-resolution Volumetric Mapping and Long-term Dynamic Scene Consistency”**, IEEE International Conference on Robotics and Automation (ICRA), 2022.
