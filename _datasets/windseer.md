---
layout: dataset
title: "WindSeer – Nature 2024 Dataset"
year: 2024
tags: [wind-estimation, environment, mapping, planning, mav, environmental-sensing]
eth_collection_url: "https://doi.org/10.3929/ethz-b-000658323"
paper: "WindSeer: Onboard Sensing and Reconstruction of Local Wind Fields for Aerial Robots (Nature 2024)"
doi: "10.3929/ethz-b-000658323"
---

The WindSeer dataset accompanies the 2024 *Nature* publication introducing a system for **onboard sensing and reconstruction of local wind fields** using micro aerial vehicles (MAVs). It contains real-world flight data, sensor readings, and reconstruction ground-truth used to evaluate the performance of the WindSeer wind-estimation and mapping framework.

This dataset enables benchmarking of:

- onboard wind-field estimation
- environmental flow reconstruction
- turbulence modeling from MAV-borne sensors
- planning and navigation under dynamic airflow conditions
- evaluation of perception–action coupling in environmental disturbances

## Data Access

➡️ **ETH Research Collection (landing page & downloads):**
**<https://doi.org/10.3929/ethz-b-000658323>**

## Contents

The dataset includes:

- Flight logs with onboard wind-sensing instrumentation
- IMU, state-estimation, and controller feedback
- Reconstructed 3D wind fields
- Ground-truth wind measurements (where available)
- Calibration information and metadata for reproducing the experimental evaluation
- Sequences from both controlled and natural outdoor environments

## Reference Paper

**WindSeer: Onboard Sensing and Reconstruction of Local Wind Fields for Aerial Robots**
Published in *Nature*, 2024.
Authors include contributors from the Autonomous Systems Lab, ETH Zürich.

<pre>
@article{windseer2024nature,
  title   = {WindSeer: Onboard Sensing and Reconstruction of Local Wind Fields for Aerial Robots},
  author  = {FirstAuthor, FirstName and SecondAuthor, FirstName and Others, et al.},
  journal = {Nature},
  year    = {2024},
  doi     = {10.3929/ethz-b-000658323},
  url     = {https://doi.org/10.3929/ethz-b-000658323}
}
</pre>