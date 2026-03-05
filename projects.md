---
layout: default
title: Projects and Competitions
permalink: /projects/
---

# Highlighted Project Works

---

## Jenga-Playing Robotic Arm

![Jenga Robot](../assets/images/projects/jenga.jpeg)

Developed an autonomous robotic manipulation system that integrates computer vision and motion planning to interact with a Jenga tower.

Key components:

- Implemented an **OpenCV-based** vision pipeline to detect, segment, and localize individual Jenga blocks.
- Designed **motion planning** strategies to identify stable blocks and perform controlled extraction without destabilizing the tower.
- Integrated **perception** and **manipulation** with the robotic arm to achieve reliable block interaction and placement.

**Project Repository:**  

<a href="https://github.com/Sairamzz/Jengics" target="_blank" class="repo-button">
<i class="fa-brands fa-github"></i> Jengics
</a>

---

## Autonomous Mobile Robot

![Autonomous Mobile Robot](../assets/images/projects/amr.jpeg)

Designed and implemented an **Autonomous Mobile Robot (AMR)** capable of mapping, localization, and navigation in indoor environments using the ROS 2 framework.

Key components:

- Built a ROS 2-based mobile robotics stack integrating **Cartographer SLAM for map generation** and **AMCL for probabilistic localization**.
- Configured the **Navigation2 framework** with global and local planners (A* / DWB) to enable goal-driven navigation with dynamic obstacle avoidance.
- Validated the system both in **Gazebo simulation and real hardware**, integrating onboard **LiDAR** sensing for **mapping** and **perception**.

**Project Repository:**  

<a href="https://github.com/Sairamzz/Autonomous-Mobile-Robot" target="_blank" class="repo-button">
<i class="fa-brands fa-github"></i> AMR
</a>

---

## APG-RRT Path Planner in ROS2

![APG RRT](../assets/images/projects/apgrrt.jpeg)

Implemented an **Adaptive Path-Guided Rapidly-Exploring Random Tree (APG-RRT)** planner for mobile robot navigation and evaluated its performance against the standard RRT algorithm.

Key components:

- Adaptive sampling-based path planning algorithm.
- Evaluated planner performance across multiple **2D benchmark environments** including long corridors, right-angle bends, and cluttered obstacle maps.
- Integrated the planner with **TurtleBot3 in Gazebo** using custom occupancy maps for navigation testing.
- Demonstrated **~25% reduction in path generation time** compared to baseline RRT while maintaining feasible navigation paths.

**Project Repository:**  

<a href="https://github.com/Sairamzz/MR_PathPlanner" target="_blank" class="repo-button">
<i class="fa-brands fa-github"></i> Path Planner Repository
</a>

---

## Structure-from-Motion (SfM) 3D Reconstruction

![SfM Reconstruction](../assets/images/projects/sfm.jpeg)

Implemented a complete **Structure-from-Motion (SfM) pipeline** to recover camera poses and reconstruct 3D scene geometry from multiple 2D images.

Key components:

- Extracted and matched visual features to establish **multi-view correspondences across image pairs**.
- Estimated relative camera motion using **epipolar geometry and incremental PnP-based pose estimation**.
- Generated 3D landmarks through **triangulation and incremental reconstruction** as additional views were registered.
- Performed **global bundle adjustment using GTSAM** to jointly optimize camera poses and 3D point estimates.
- Evaluated reconstruction accuracy by comparing intrinsic parameters and results against **COLMAP calibration outputs**.

**Project Repository:**  

<a href="https://github.com/Sairamzz/Structure_From_Motion" target="_blank" class="repo-button">
<i class="fa-brands fa-github"></i> SfM Pipeline Repository
</a>

---

## Camera–LiDAR Extrinsic Calibration (On-the-Fly)

![Camera LiDAR Calibration](../assets/images/projects/calibration.jpeg)

Developed a pipeline to estimate the **6-DoF extrinsic transformation between camera and LiDAR sensors** during runtime using geometric feature alignment.

Key components:

- Processed synchronized LiDAR point clouds and camera images to extract **depth discontinuities and visual edge features**.
- Identified corresponding geometric structures using **KD-Tree search and Canny edge detection**.
- Optimized the camera-LiDAR transform using **grid search and pose refinement**.
- Validated calibration quality through **edge overlay visualization, robustness tests with injected offsets, and quantitative alignment metrics**.

**Project Repository:**  

<a href="https://github.com/Sairamzz/Camera-Lidar-Extrinsic-Calibration-On-the-fly" target="_blank" class="repo-button">
<i class="fa-brands fa-github"></i> Calibration Repository
</a>
