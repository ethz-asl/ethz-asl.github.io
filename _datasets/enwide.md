---
layout: dataset
title: "ENWIDE LiDAR Inertial Dataset"
year: 2024
tags: [mapping, lidar, odometry, slam, degeneracy, outdoor, indoor]
eth_collection_url: "http://hdl.handle.net/20.500.11850/787551"
paper: "COIN-LIO: Complementary Intensity-Augmented LiDAR Inertial Odometry"
doi: "10.3929/ethz-c-000787551"
featured: true
---

# ENWIDE LiDAR Inertial Dataset

This page contains the data and information for the LiDAR Inertial dataset in **en**vironments **wi**th large sections
of **de**generate geometry that was presented in the ICRA 2024 publication COIN-LIO.


---

## Data Access

➡️ **ETH Research Collection (landing page & downloads):**
**<https://doi.org/10.3929/ethz-c-000787551>**

---

## Dataset Description

The dataset was recorded using an **Ouster OS0 128 (Rev D) LiDAR** at **10 Hz** with **1024×128 points** per revolution.
The IMU data is recorded at **100 Hz** using the internal IMU of the LiDAR.

The ground-truth position was recorded from a **Leica MS60 Total Station** using a prism mounted on top of the LiDAR and time-synced accordingly.

The sensor was carried on a handheld stick. For each environment, one **smooth** (walking, slow motions) and one **dynamic** (running, aggressive motions) sequence is provided, indicated by "**s**" or "**d**" at the end of the filename:
Example: `2023-08-08-17-50-31-tunnel_d.bag`

Sequences are provided as **rosbags**, and ground truth files are provided as **CSV in TUM format**.

---

## Prism Extrinsics

IMU-to-prism extrinsics (CAD-derived) are available here:
[prism_imu_extrinsics.txt](http://robotics.ethz.ch/~asl-datasets/2024_ICRA_ENWIDE/prism_imu_extrinsics.txt)

![LiDAR pole](/assets/datasets/enwide/lidar_pole.jpeg)

---

## Environments

Exemplary images of each environment, along with manually annotated starting positions:

### **Intersection**
![Intersection](/assets/datasets/enwide/intersecion_prev.jpg)
[Location](https://maps.app.goo.gl/v4bSYDYEaMte7j4p7)

### **Runway**
![Runway](/assets/datasets/enwide/runway_prev.jpg)
[Location](https://maps.app.goo.gl/BdCSKbcpqRzKcr4w6)

### **Field**
![Field](/assets/datasets/enwide/field_prev.png)
[Location](https://maps.app.goo.gl/s1fBBs1kN4bfWJc59)

### **Tunnel**
![Tunnel](/assets/datasets/enwide/tunnel_prev.jpg)
[Location](https://maps.app.goo.gl/vKyPvk5QTkdoCSiR8)

### **Katzensee**
![Katzensee](/assets/datasets/enwide/katzensee_prev.jpg)
[Location](https://maps.app.goo.gl/pWw73NwZJ9UMDffM7)

## Reference Paper
**COIN-LIO: Complementary Intensity-Augmented LiDAR Inertial Odometry**
IEEE International Conference on Robotics and Automation (ICRA), 2024.

<pre>
@inproceedings{pfreundschuh2024coin,
  title={Coin-lio: Complementary intensity-augmented lidar inertial odometry},
  author={Pfreundschuh, Patrick and Oleynikova, Helen and Cadena, Cesar and Siegwart, Roland and Andersson, Olov},
  booktitle={2024 IEEE International Conference on Robotics and Automation (ICRA)},
  pages={1730--1737},
  year={2024},
  organization={IEEE}
}
</pre>