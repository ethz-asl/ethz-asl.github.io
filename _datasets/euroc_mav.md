---
title: "EuRoC MAV Dataset"
paper: "The EuRoC micro aerial vehicle datasets, IJRR 2016"
citation: "M. Burri et al., IJRR, 2016"
year: 2016
tags: [visual-inertial, MAV, SLAM]
doi: "10.3929/ethz-b-000690084"
eth_collection_url: "https://doi.org/10.3929/ethz-b-000690084"
featured: true        # ← star this one
layout: dataset
---

![ETH Machine Hall](/assets/datasets/euroc/overview_ml.jpg)
![Vicon Training](/assets/datasets/euroc/vicon_pointcloud_training_crop.png)



This page presents visual-inertial datasets collected on-board a micro aerial vehicle (MAV).
The datasets contain stereo images, synchronized IMU measurements, and accurate motion and structure ground-truth.

## Publication

M. Burri, J. Nikolic, P. Gohl, T. Schneider, J. Rehder, S. Omari, M. Achtelik, R. Siegwart,
**The EuRoC micro aerial vehicle datasets**, International Journal of Robotic Research, 2016.
[Publisher link](https://doi.org/10.1177/0278364915620033)

<details>
<summary><strong>BibTeX Citation</strong></summary>

<pre>
@article{Burri25012016,
  author  = {Burri, Michael and Nikolic, Janosch and Gohl, Pascal and Schneider, Thomas and Rehder, Joern and Omari, Sammy and Achtelik, Markus W and Siegwart, Roland},
  title   = {The EuRoC micro aerial vehicle datasets},
  year    = {2016},
  doi     = {10.1177/0278364915620033},
  URL     = {http://ijr.sagepub.com/content/early/2016/01/21/0278364915620033.abstract},
  eprint  = {http://ijr.sagepub.com/content/early/2016/01/21/0278364915620033.full.pdf+html},
  journal = {The International Journal of Robotics Research}
}
</pre>
</details>

## Downloads

> All dataset files are now hosted on the ETH Research Collection.

- **Dataset landing page**: [ETH Research Collection]({{ page.eth_collection_url }})

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
