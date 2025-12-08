---
layout: dataset
title: "Dynablox: Real-time Detection of Diverse Dynamic Objects in Complex Environments"
year: 2023
tags: [lidar, dynamic-objects, indoor, outdoor]
eth_collection_url: "http://hdl.handle.net/20.500.11850/788607"
paper: "L. Schmid, O. Andersson, A. Sulser, P. Pfreundschuh, R. Siegwart, “Dynablox: Real-time Detection of Diverse Dynamic Objects in Complex Environments”, IEEE Robotics and Automation Letters (RA-L), Vol. 8, No. 10, pp. 6259-6266, 2023."
doi: "10.3929/ethz-c-000788607"
---

This dataset supports the research system *Dynablox*, designed for incremental mapping-based detection of diverse moving objects in complex indoor and outdoor environments.
The corresponding code is available at [https://github.com/ethz-asl/dynablox](https://github.com/ethz-asl/dynablox) and the paper is available on arXiv and IEEE.

![Example dynamic object scene](/assets/datasets/dynablox/dynablox_data.png)

## Dataset Description

The Dynablox dataset consists of multiple sequences collected using a 128-beam OS0 high-range, high-resolution LiDAR sensor. It features a wide variety of dynamic objects including typical entities (e.g., pedestrians) and atypical motion events (e.g., tossed or bounced balls, luggage rolling down ramps, people occluded behind large objects like boxes or surfboards). The scenes cover both indoor and outdoor settings with clutter, stairs, ramps, and multi-level structures. :contentReference[oaicite:1]{index=1}

## Data Layout

We provide eight base sequences (via ROS bags) covering the following scenarios:
- corridor_1
- corridor_2
- hg_1
- h_2
- indoor
- ramp_1
- ramp_2
- stairs

For each sequence there are two archive versions available:
- **Raw**: original point clouds, IMU data, and an onboard visual-inertial (VI) state estimate.
- **Processed**: state estimates from FAST‑LIO2, undistorted point clouds (for points with available state estimates), and typically the first second of data removed to allow FAST-LIO2 to stabilise. :contentReference[oaicite:3]{index=3}

## Downloads
Available via the ETH Research Collection (see DOI link above).

## Use Cases & Applications

- Real-time detection and tracking of dynamic objects in 3D LiDAR data
- Testing of object-aware mapping, segmentation, and planning in mixed stationary/dynamic environments
- Benchmarking of perception pipelines for indoor/outdoor mobility platforms

## Citation

> L. Schmid, O. Andersson, A. Sulser, P. Pfreundschuh, R. Siegwart,
> **“Dynablox: Real-time Detection of Diverse Dynamic Objects in Complex Environments”**, IEEE Robotics and Automation Letters (RA-L), Vol. 8, No. 10, pp. 6259-6266, 2023.
