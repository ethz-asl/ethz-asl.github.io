---
layout: dataset
title: "Dynamic Object Aware LiDAR SLAM Dataset"
year: 2021
tags: [lidar, dynamic-objects, slam, urban, outdoor]
eth_collection_url: ""
paper: "P. Pfreundschuh, H. F. C. Hendrikx, V. Reijgwart, R. Dubé, R. Siegwart, A. Cramariuc, “Dynamic Object Aware LiDAR SLAM based on Automatic Generation of Training Data”, IEEE International Conference on Robotics and Automation (ICRA), 2021."
doi: ""
---

Urban handheld LiDAR dataset (Ouster OS1-64, 10 Hz) with dynamic object annotations for SLAM evaluation across ETH Zurich main hall, Zurich train station (two levels), and a pedestrian zone, plus a simulated town sequence with full ground truth.

![ETH main hall annotated](/assets/datasets/doals/hauptgebaeude_annotated_small.png)
![Niederdorf annotated](/assets/datasets/doals/niederdorf_annotated_small.png)
![Shopville annotated](/assets/datasets/doals/shopville_annotated_small.png)
![Station annotated](/assets/datasets/doals/station_annotated_small.png)

## Dataset Description

- 8 real-world sequences (100–400 m, 100–200 s) with high-frequency VI-SLAM poses
- Annotated dynamic objects (pedestrians and associated items) for 10 temporally separated clouds per sequence (`indices.csv` per sequence)
- Simulated town sequence with moving vehicles/pedestrians/objects and full ground-truth poses/annotations
- Sensor: Ouster OS1-64 Gen1, 2048 pts/rev

## Topics

- `/os1_cloud_node/points` — `sensor_msgs/PointCloud2`
- `/tf` — `tf2_msgs/TFMessage`
- `/T_map_os1_lidar` or `/T_map_os1_sensor` — `geometry_msgs/TransformStamped`

Use provided poses to undistort handheld scans.

## Downloads

- Dataset directory: **Research Collection link pending** (was `2021_ICRA_dynamic_object_lidar_dataset/scenes`)

## Citation

> P. Pfreundschuh, H. F. C. Hendrikx, V. Reijgwart, R. Dubé, R. Siegwart, A. Cramariuc,  
> **“Dynamic Object Aware LiDAR SLAM based on Automatic Generation of Training Data”**, IEEE International Conference on Robotics and Automation (ICRA), 2021.
