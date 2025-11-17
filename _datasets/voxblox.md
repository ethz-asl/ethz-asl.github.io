---
layout: dataset
title: "IROS 2017 – Voxblox Dataset"
year: 2017
tags: [tsdf, esdf, mapping, reconstruction, planning, mav]
eth_collection_url: "https://doi.org/10.3929/ethz-b-000721636"
paper: "Helen Oleynikova, Zachary Taylor, Markus Fehr, Juan Nieto, Roland Siegwart – Voxblox: Incremental 3D Euclidean Signed Distance Fields for On-Board MAV Planning (IROS 2017)"
doi: "10.3929/ethz-b-000721636"
---

![Cow & Lady](/assets/datasets/voxblox/scene_photo.jpg)


This dataset accompanies the **Voxblox** 3D volumetric mapping system, released in conjunction with the IROS 2017 paper *“Voxblox: Incremental 3D Euclidean Signed Distance Fields for On-board MAV Planning.”*

It provides RGB-D and/or depth-only sequences suitable for **TSDF/ESDF reconstruction**, **incremental mapping**, and **robotic planning** evaluation.

Original dataset page:
https://projects.asl.ethz.ch/datasets/doku.php?id=iros2017

## Data Access

The dataset is now permanently hosted on the ETH Research Collection:

➡️ **Download / Landing Page:**
**<https://doi.org/10.3929/ethz-b-000721636>**

## Contents

The dataset includes sequences used for evaluating:

- voxel-based TSDF reconstruction
- incremental ESDF generation
- planning-aware mapping
- online MAV/local robot navigation

Typical data provided:

- RGB–D recordings
- depth images
- calibrated intrinsic/extrinsic parameters
- ground-truth or reference reconstructions (in some sequences)
- example output reconstructions from Voxblox

## Paper

**Voxblox: Incremental 3D Euclidean Signed Distance Fields for On-board MAV Planning**
Helen Oleynikova, Zachary Taylor, Markus Fehr, Juan Nieto, Roland Siegwart
*IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2017.*

GitHub: https://github.com/ethz-asl/voxblox

## BibTeX

<pre>
@inproceedings{oleynikova2017voxblox,
  title        = {Voxblox: Incremental {3D} Euclidean Signed Distance Fields for On-Board {MAV} Planning},
  author       = {Oleynikova, Helen and Taylor, Zachary and Fehr, Markus and Nieto, Juan and Siegwart, Roland},
  booktitle    = {2017 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  pages        = {1366--1373},
  year         = {2017},
  organization = {IEEE}
}
</pre>