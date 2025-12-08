---
layout: dataset
title: "MultiPoint: Cross-spectral Optical–Thermal Aerial Imagery"
year: 2020
tags: [aerial, multispectral, thermal, optical, registration]
eth_collection_url: "http://hdl.handle.net/20.500.11850/788340"
paper: "F. Achermann, A. Kolobov, D. Dey, T. Hinzmann, J. J. Chung, R. Siegwart, N. Lawrance, “MultiPoint: Cross-spectral registration of thermal and optical aerial imagery”, Conference on Robot Learning (CoRL), 2020."
doi: "10.3929/ethz-c-000788340"
---

Aligned optical–thermal image pair dataset from fixed-wing UAV flights for cross-spectral registration. Captured with a UI-5261SE RGB camera (16 mm) and FLIR TAU2 19 mm (7.5–13.5 μm).

![Sample aligned optical/thermal pair](/assets/datasets/corl2020_multipoint/altair-sample-1.gif)

## Dataset Description

- 10 flights at varying times of day; split into training and test sets
- HDF5 samples with three aligned images: `optical`, `thermal`, `thermal_raw`
  - 640×512 resolution, undistorted and aligned
  - Optical: grayscale normalized [0,1]
  - Thermal: normalized per-image (1st–99th percentile)
  - Thermal raw normalized by 16383; temperature °C = `pixel_val * 16383 * 0.04 - 273.15`
- Loader interface available in [multipoint](https://github.com/ethz-asl/multipoint)

## Downloads

- Training set (24 GB, 9340 pairs): **Research Collection link pending** (was `training.hdf5`)
- Test set (12 GB, 4391 pairs): **Research Collection link pending** (was `test.hdf5`)
- Training keypoint labels (10 MB): **Research Collection link pending** (was `labels_training.hdf5`)

## Citation

> F. Achermann, A. Kolobov, D. Dey, T. Hinzmann, J. J. Chung, R. Siegwart, N. Lawrance,  
> **“MultiPoint: Cross-spectral registration of thermal and optical aerial imagery”**, Conference on Robot Learning (CoRL), 2020.
