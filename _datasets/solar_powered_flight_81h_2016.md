---
layout: dataset
title: "AtlantikSolar 81-hour Solar-powered Flight Dataset"
year: 2016
tags: [uav, solar, endurance, flight-data]
eth_collection_url: "https://doi.org/10.3929/ethz-c-000787517"
paper: "P. Oettershagen, A. Melzer, T. Mantel, K. Rudin, T. Stastny, B. Wawrzacz, T. Hinzmann, S. Leutenegger, K. Alexis, R. Siegwart, “Design of small hand-launched solar-powered UAVs: From concept study to a multi-day world endurance record flight”, Journal of Field Robotics (JFR), 2016."
doi: "10.3929/ethz-c-000787517"
---

Pixhawk log dataset from the 81-hour continuous solar-powered flight (July 14–17, 2015) by the AtlantikSolar UAV, including power system telemetry and controller data for endurance analysis.

![AtlantikSolar aircraft](/assets/datasets/solar_powered_flight_81h_2016/atlantiksolar_aircraft.jpg)

## Dataset Information

- Logged via Pixhawk (sdlog2), ~2 Hz, 645k entries over 296,074 seconds
- Events (approx. local time): log start 09:08, launch 09:32 (July 14); landing 18:56 (July 17); log end 19:20
- Custom firmware based on PX4 commit `97a1410` (Nov 12, 2014)
- Contains flight controller states/references, power system readings (MPPT, power sensors, battery monitors), atmospheric temperature, and autopilot configuration parameters

Refer to the original page for detailed field definitions (ASLCTRL, MPPT, battery monitors, atmospheric sensors).

## Download

- Full dataset (.mat in zip): <https://doi.org/10.3929/ethz-c-000787517>

## Citation

> P. Oettershagen, A. Melzer, T. Mantel, K. Rudin, T. Stastny, B. Wawrzacz, T. Hinzmann, S. Leutenegger, K. Alexis, R. Siegwart,  
> **“Design of small hand-launched solar-powered UAVs: From concept study to a multi-day world endurance record flight”**, Journal of Field Robotics (JFR), 2016.
