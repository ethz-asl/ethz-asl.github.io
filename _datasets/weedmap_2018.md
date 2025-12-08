---
layout: dataset
title: "WeedMap: Large-scale Multispectral Weed Mapping Dataset"
year: 2018
tags: [agriculture, multispectral, semantic-segmentation, orthomosaic, uav]
eth_collection_url: "https://doi.org/10.3929/ethz-c-000788571"
paper: "I. Sa, M. Popovic, R. Khanna, Z. Chen, P. Lottes, F. Liebisch, J. Nieto, C. Stachniss, A. Walter, R. Siegwart, “WeedMap: A large-scale semantic weed mapping framework using aerial multispectral imaging and deep neural network for precision farming”, Remote Sensing, 2018."
doi: "10.3929/ethz-c-000788571"
---

Multispectral UAV dataset over sugar beet fields in Eschikon (Switzerland) and Rheinbach (Germany) with orthomosaic maps and tiled crops for weed/crop segmentation. Captured with MicaSense RedEdge-M and Sequoia cameras.

![WeedMap overview](/assets/datasets/weedmap_2018/dataset-page.png)
![WeedMap flight path](/assets/datasets/weedmap_2018/flight-path.png)

## Highlights

- 8 datasets (indices 000–007), 18,746 images across 129 directories (~5.36 GB)
- Orthomosaics and tiles with RGB/CIR/NDVI composites, masks, and pixel-level labels
- Ground truth: background/crop/weed (color and indexed label maps)
- Flight paths provide ~1 cm GSD; includes interactive viewers for orthomosaics
- Camera specs and folder structure docs included; MATLAB scripts for tile/orthomosaic conversion

## Folder Structure

- `Orthomosaic/RedEdge` and `Orthomosaic/Sequoia`: composite PNG, groundtruth labels, reflectance TIFFs
- `Tiles/RedEdge` and `Tiles/Sequoia`: per-channel tiles, masks, and groundtruth labels
- Naming: `XXX_frameYYYY_GroundTruth_color.png` / `..._iMap.png`, masks `frameYYYY`, tiles per channel

## Downloads

- Full dataset (5.36 GB): <https://doi.org/10.3929/ethz-c-000788571>
- Orthomosaics:
  - RedEdge bundle (1.9 GB): <https://doi.org/10.3929/ethz-c-000788571>
  - Sequoia bundle (1.49 GB): <https://doi.org/10.3929/ethz-c-000788571>
  - Per-dataset archives 000–007 available (links to be updated)
- Tiles:
  - RedEdge bundle (637 MB): <https://doi.org/10.3929/ethz-c-000788571>
  - Sequoia bundle (444 MB): <https://doi.org/10.3929/ethz-c-000788571>
  - Per-dataset archives 000–007 available (links to be updated)

## Citation

> I. Sa, M. Popovic, R. Khanna, Z. Chen, P. Lottes, F. Liebisch, J. Nieto, C. Stachniss, A. Walter, R. Siegwart,  
> **“WeedMap: A large-scale semantic weed mapping framework using aerial multispectral imaging and deep neural network for precision farming”**, Remote Sensing, 2018. DOI: 10.3390/rs10091423.
