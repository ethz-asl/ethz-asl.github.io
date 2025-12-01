---
layout: dataset
title: "Eschikon Plant Stress Phenotyping Dataset"
year: 2019
tags: [agriculture, multispectral, plant-stress, field]
eth_collection_url: ""
paper: "R. Khanna, L. Schmidt, J. Nieto, R. Siegwart, F. Liebisch, “A Spatio Temporal Spectral Dataset for Plant Stress Phenotyping”, Plant Methods, 2019."
doi: ""
---

Spatio-temporal-spectral dataset of sugar beet crop growth under drought, fertilizer, and weed stress over two months in Eschikon, Switzerland. Includes biweekly RGB images, infrared stereo pairs, multispectral images, treatment parameters, and environmental logs.

![Dataset overview](/assets/datasets/plant_stress_phenotyping_2018/dataset-overview.jpg)

## Treatments at a Glance

Multiple box-level treatments with combinations of soil type, water input, nitrogen level, and weed pressure (control, low/med/high N, weed-only variants, drying, mixed stress). See treatment table in dataset for box indices and conditions.

## Contents

- Images: biweekly RGB, infrared stereo, multispectral (organized by date and camera)
- Spectral point clouds: MATLAB `.mat` format
- Calibration images (checkerboards)
- Greenhouse temperature/humidity logs
- Box weight measurements (soil moisture proxy)
- SPAD measurements
- Above/below ground biomass (yield indicators)

Processing utilities: [plant_stress_phenotyping](https://github.com/ethz-asl/plant_stress_phenotyping)

## Downloads

- Dataset root: **Research Collection link pending** (was `2018_plant_stress_phenotyping_dataset/`)
- Images (2.5 GB): **Research Collection link pending** (was `images.zip`)
- Point clouds (2.5 GB): **Research Collection link pending** (was `pointclouds.zip`)
- Calibration: **Research Collection link pending** (was `calibration.zip`)
- Greenhouse logs: **Research Collection link pending** (was `greenhouse-temperature-humidity-logs.csv`)
- Box weights: **Research Collection link pending** (was `box-weights-kg.csv`)
- SPAD: **Research Collection link pending** (was `spad-measurements.csv`)
- Yield weights: **Research Collection link pending** (was `yield-weight-grams.csv`)

## Citation

> R. Khanna, L. Schmidt, J. Nieto, R. Siegwart, F. Liebisch,  
> **“A Spatio Temporal Spectral Dataset for Plant Stress Phenotyping”**, Plant Methods, 2019.
