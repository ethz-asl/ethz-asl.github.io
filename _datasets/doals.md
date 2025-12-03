---
layout: dataset
title: "Urban Dynamic Objects LiDAR Dataset"
year: 2021
tags: [mapping, lidar, dynamic, pedestrian, slam, urban, outdoor]
eth_collection_url: "http://hdl.handle.net/20.500.11850/788171"
paper: "Dynamic Object Aware LiDAR SLAM based on Automatic Generation of Training Data"
doi: "10.3929/ethz-c-000788171"
featured: true
---

# Urban Dynamic Objects LiDAR Dataset

![Hauptgebaeude](/assets/datasets/doals/hauptgebaeude_annotated_small.png)
![Niederdorf](/assets/datasets/doals/niederdorf_annotated_small.png)
![Shopville](/assets/datasets/doals/shopville_annotated_small.png)
![Station](/assets/datasets/doals/station_annotated_small.png)


## Data Access

➡️ **ETH Research Collection (landing page & downloads):**
**<https://doi.org/10.3929/ethz-c-000788171>**

---

## Dataset Description

The dataset contains **more than 12,000 scans** recorded in:

- The main hall of ETH Zurich (**Hauptgebaeude**)
- Two levels of Zurich main train station (**Station**, **Shopville**)
- A touristic pedestrian zone (**Niederdorf**)

Each location includes **2 sequences**.
The point clouds include a significant number of pedestrians.

Data was recorded using a **handheld Ouster OS1 64 (Gen 1) LiDAR** at **10 Hz** with **2048 points per revolution**.

We provide **globally bundle-adjusted high-frequency poses** from a VI-SLAM pipeline.
Trajectory lengths range from **100–400 m**, and sequence durations are **100–200 s**.

### Annotations

A subset of the dataset was manually annotated:

- 10 temporally separated point clouds per sequence (8 sequences total)
- Pedestrians and objects associated with them (suitcases, bicycles, dogs, etc.)
- Annotation was based on **appearance only** (not motion state)

### Simulated Dataset

We additionally provide a simulated sequence of a small town featuring:

- Moving **cars, planes, pedestrians, animals**
- **Cylinders, spheres, cubes** of varying sizes
- Objects moving horizontally and vertically at different velocities
- A simulated LiDAR (similar to OS1 64 Gen 1) moving along a closed trajectory
  → Ground truth poses and object annotations available for all point clouds

---

## Structure of the Dataset

Sequences are provided as **rosbag** files.

### Topics

| Description       | Topic                          | Message Type                      |
|-------------------|--------------------------------|-----------------------------------|
| Point Clouds      | `/os1_cloud_node/points`       | `sensor_msgs/PointCloud2`         |
| Transformations   | `/tf`                           | `tf2_msgs/TFMessage`              |
| Transformations   | `/T_map_os1_lidar` or `/T_map_os1_sensor` | `geometry_msgs/TransformStamped`  |

The world coordinate frame is **`map`**.
Point clouds are recorded in:

- `os1_lidar` frame (real datasets)
- `os1_sensor` frame (simulated dataset)

Corresponding poses are provided via `/tf` or `/T_map_os1_lidar(sensor)`.

### Distortion & Undistortion

Because the sensor was handheld, point clouds are distorted by ego motion.
The provided high-frequency poses can be used for undistortion.

### Dynamic Object Indices

For each sequence, annotated dynamic objects are stored in an **`indices.csv`** file:

- Each line begins with the **timestamp (ns)** of the point cloud
- Followed by all **annotated dynamic point indices**

---

## Reference Paper
Patrick Pfreundschuh, Hubertus F.C. Hendrikx, Victor Reijgwart, Renaud Dubé, Roland Siegwart, Andrei Cramariuc,
*Dynamic Object Aware LiDAR SLAM based on Automatic Generation of Training Data*,
IEEE International Conference on Robotics and Automation (ICRA), 2021.

<pre>
@inproceedings{pfreundschuh2021dynamic,
  title={Dynamic object aware lidar slam based on automatic generation of training data},
  author={Pfreundschuh, Patrick and Hendrikx, Hubertus FC and Reijgwart, Victor and Dub{\'e}, Renaud and Siegwart, Roland and Cramariuc, Andrei},
  booktitle={2021 IEEE International Conference on Robotics and Automation (ICRA)},
  pages={11641--11647},
  year={2021},
  organization={IEEE}
}
</pre>