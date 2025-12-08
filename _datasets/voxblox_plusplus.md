---
layout: dataset
title: "Volumetric Instance-Aware Semantic Mapping and 3D Object Discovery"
year: 2019
tags: [rgbd, mapping, semantic, instance, indoor]
eth_collection_url: "http://hdl.handle.net/20.500.11850/788341"
paper: "M. Grinvald, F. Furrer, T. Novkovic, J. J. Chung, C. Cadena, R. Siegwart, J. Nieto, “Volumetric Instance-Aware Semantic Mapping and 3D Object Discovery”, IEEE Robotics and Automation Letters (RA-L), 2019."
doi: "10.3929/ethz-c-000788341"
---

RGB-D rosbags for the Voxblox++ (Volumetric Instance-Aware Semantic Mapping) paper, including a SceneNN sequence and an office-floor run with multiple depth/RGB streams for online mapping experiments.

![Semantic instance-aware map](/assets/datasets/voxblox_plusplus/mobmi00.png)

## Dataset Details

- **SceneNN 231**: 3:06 duration, 7.9 GB; topics include RGB-D images, camera info, TF
- **Office floor (ASL)**: 5:12 duration, 6.3 GB; two Primesense cameras (front/table) with depth_registered and RGB streams; high-frequency TF
- Suitable for semantic/instance-aware volumetric mapping and object discovery benchmarks

## Downloads

- SceneNN sequence: <http://hdl.handle.net/20.500.11850/788341> (was `scenenn_231.bag`, 7.9 GB)
- Office floor sequence: <http://hdl.handle.net/20.500.11850/788341> (was `asl_office_floor.bag`, 6.3 GB)

## Citation

> M. Grinvald, F. Furrer, T. Novkovic, J. J. Chung, C. Cadena, R. Siegwart, J. Nieto,  
> **“Volumetric Instance-Aware Semantic Mapping and 3D Object Discovery”**, IEEE Robotics and Automation Letters (RA-L), 2019.
