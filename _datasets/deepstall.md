---
layout: dataset
title: "In-Wing Pressure Measurements for Airspeed and Airflow Angle Estimation"
year: 2022
tags: [uav, aerodynamics, sensing, pressure, flight]
eth_collection_url: "http://hdl.handle.net/20.500.11850/788334"
paper: "G. A. Heinrich, S. Vogt, N. R. Lawrance, T. J. Stastny, R. Y. Siegwart, “In-Wing Pressure Measurements for Airspeed and Airflow Angle Estimation and High Angle-of-Attack Flight”, Journal of Guidance, Control, and Dynamics, 2022."
doi: "10.3929/ethz-c-000788334"
---

Hardware designs and datasets for in-wing differential pressure sensing on a small UAV (EasyGlider 4), covering wind tunnel and flight tests for airspeed and airflow angle estimation and deep stall/high angle-of-attack maneuvers. Preview imagery and PCB/STEP files to be rehosted with the dataset.

## Dataset Description

- HDF5 logs for **raw** and **calibrated** data, each with wind tunnel and flight datasets
- Includes PX4-based navigation data (ulog), synchronized at 40 Hz with preliminary airspeed estimates
- Calibrated datasets provide airspeed, airflow angles, and current following the paper’s procedure
- Key fields include differential pressures, airspeed, angles of attack/sideslip, vehicle attitude, and PX4 state
- Example Python script for reading/plotting; MATLAB HDF5 tools also applicable

## Hardware Designs

- Differential pressure module STEP files
- PCB designs as KiCAD projects

## Downloads

- Full dataset (3.0 GB): **Research Collection link pending** (was `Data_Deep_Stall.7z`)
- STEP files (6.6 MB): **Research Collection link pending** (was `dp_module_step_files.zip`)
- KiCAD projects (2.0 MB): **Research Collection link pending** (was `KiCad.zip`)

## Citation

> G. A. Heinrich, S. Vogt, N. R. Lawrance, T. J. Stastny, R. Y. Siegwart,  
> **“In-Wing Pressure Measurements for Airspeed and Airflow Angle Estimation and High Angle-of-Attack Flight”**, Journal of Guidance, Control, and Dynamics, 2022. DOI: 10.2514/1.G006412.
