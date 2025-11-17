---
title: "EuRoC MAV Dataset"
paper: "The EuRoC micro aerial vehicle datasets, IJRR 2016"
citation: "M. Burri et al., IJRR, 2016"
year: 2016
tags: [visual-inertial, MAV, SLAM]
doi: "10.3929/ethz-b-000XXXXX"   # replace with actual ETH Research Collection DOI
eth_collection_url: "https://www.research-collection.ethz.ch/handle/20.500.11850/XXXXX"
layout: dataset                  # we’ll make this layout in a second
---

![ETH Machine Hall](/assets/datasets/euroc/overview_ml.jpg)
![Vicon Training](/assets/datasets/euroc/vicon_pointcloud_training_crop.png)



This page presents visual-inertial datasets collected on-board a micro aerial vehicle (MAV).
The datasets contain stereo images, synchronized IMU measurements, and accurate motion and structure ground-truth.

## Publication

M. Burri, J. Nikolic, P. Gohl, T. Schneider, J. Rehder, S. Omari, M. Achtelik, R. Siegwart,
**The EuRoC micro aerial vehicle datasets**, International Journal of Robotic Research, 2016.
[Publisher link](https://doi.org/10.1177/0278364915620033)
[BibTeX](link-to-bibtex-file-or-anchor)

## Downloads

> All dataset files are now hosted on the ETH Research Collection.

- **Dataset landing page**: [ETH Research Collection]({{ page.eth_collection_url }})
- (Optional) Direct links to common formats (if the Collection gives stable URLs):
  - ROS bags
  - “ASL Dataset Format” archives

## Available Data

- **Visual-inertial sensor unit**
  - Stereo images (WVGA monochrome, 2×20 FPS)
  - MEMS IMU (angular rate and acceleration, 200 Hz)
  - Shutter-centric temporal alignment
- **Ground-truth**
  - Vicon motion capture system (6D pose)
  - Leica MS50 laser tracker (3D position)
  - Leica MS50 3D structure scan
- **Calibration**
  - Camera intrinsics
  - Camera–IMU extrinsics
  - Spatio-temporally aligned ground truth

![Platform](/assets/datasets/euroc/platform.jpg)
![Sensor Setup](/assets/datasets/euroc/sensor_setup2.png)


## Tools

- Dataset parser: [dataset_tools](https://github.com/ethz-asl/dataset_tools)

## Known issues

- The visual-inertial sensor uses automatic exposure control independently per camera, leading to varying brightness between the stereo pair.
- Some datasets exhibit very dynamic motions that can deteriorate laser tracker accuracy.
- Synchronization between sensor data and motion ground truth is limited by separate recording systems and missing device timestamps for Vicon; see the paper for details.
