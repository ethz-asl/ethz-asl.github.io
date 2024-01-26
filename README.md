# About the Autonomous Systems Lab
The [Autonomous Systems Lab](http://www.asl.ethz.ch/) is part of the Mechanical Engineering department at ETH Zurich, under Prof. Roland Siegwart.

The main focus of the lab is autonomous robotic systems, including hardware, state estimation, perception, and planning.
A small subset of the software packages we've made available open-source are listed and described here.

# Open-Source Projects
These projects are divided by general area. Note that not all of these are appropriate for every robot or application, please read each package's individual documentation.



## State Estimation
[maplab](https://github.com/ethz-asl/maplab) -- Research-oriented visual-inertial mapping framework, written in C++, for creating, processing and manipulating multi-session maps. On the one hand, maplab can be considered as a ready-to-use visual-inertial mapping and localization system. On the other hand, maplab provides a collection of multi-session mapping tools that include map merging, visual-inertial batch optimization, and loop closure.

[rovio](https://github.com/ethz-asl/rovio) -- Robust Visual Inertial Odometry framework, estimating the pose of a robot based on synchronized IMU and monocular or stereo camera input. EKF-based.

[ethzasl_msf](https://github.com/ethz-asl/ethzasl_msf) -- Multi-sensor fusion, allowing fusing multiple sensors estimating a robots' pose together, such as multiple IMUs, IMU and camera pose estimates, external position tracking estimates, etc. Compensates for sensor delays.



## Perception
[wavemap](https://github.com/ethz-asl/wavemap) -- Fast, efficient and accurate multi-resolution, multi-sensor 3D occupancy mapping.

[libpointmatcher](https://github.com/ethz-asl/libpointmatcher) -- A library implementing various ICP (Iterative Closest Point) algorithms for laser and other scan matching in 3D. A ROS wrapper is available at [ethzasl_icp_mapping](https://github.com/ethz-asl/ethzasl_icp_mapping).

[volumetric_mapping](https://github.com/ethz-asl/volumetric_mapping) -- Wrapper around Octomap, allowing input from various data sources (such as disparity maps) and a more flexible sensor position interface. 
[grid_map](https://github.com/ethz-asl/grid_map) -- 2.5 D grid-based mapping with multiple layers for robot navigation.

[elevation_mapping](https://github.com/ethz-asl/elevation_mapping) -- Local elevation mapping, expressed in a robot-centric frame for navigation, especially for walking robots.

## Calibration
[kalibr](https://github.com/ethz-asl/kalibr) -- Camera and IMU calibration toolbox.

## Planning
[StructuralInspectionPlanner](https://github.com/ethz-asl/StructuralInspectionPlanner) -- Toolbox for planning paths for a flying robot to inspect a structure for which a mesh representation is known.


## Simulation
[rotors_simulator](https://github.com/ethz-asl/rotors_simulator) -- Gazebo-based simulator for multirotor helicopters and quadrotors. Provides physical models, sensor models, octomap generation from Gazebo world, and realistic aerodynamics simulation.

## Mathematics
[minkindr](https://github.com/ethz-asl/minkindr) -- Lightweight, simple transformation library, handling Quaternion-based transformations. Conversions to/from ROS are available as part of the [minkindr_ros](https://github.com/ethz-asl/minkindr_ros) package.

## Hardware Interfaces/Drivers
[visensor_node](https://github.com/ethz-asl/visensor_node), [libvisensor](https://github.com/ethz-asl/libvisensor) -- Drivers for the VI Sensor, a sensor with a stereo head synchronized to an IMU.

[VersaVIS](https://github.com/ethz-asl/versavis) -- Provides a complete, open-source hardware, firmware and software bundle to perform time synchronization of multiple cameras with an IMU featuring exposure compensation, host clock translation and independent and stereo camera triggering.
