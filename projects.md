---
layout: default
title: Projects and Competitions
permalink: /projects/
---

# Highlighted Project Works

---

## Jenga-Playing Robotic Arm

![Jenga Robot](../assets/images/projects/jenga.jpeg)

Developed a robotic manipulation system capable of **playing Jenga autonomously** using computer vision and motion planning.

Key components:

- Implemented **OpenCV-based perception** for detecting and localizing Jenga blocks.
- Designed algorithms for **safe block extraction and placement**.
- Integrated perception and control with the robotic arm to perform **precise manipulation tasks**.

**Repository:**  
[Jengics GitHub](https://github.com/Sairamzz/Jengics)

---

## Autonomous Mobile Robot

![Autonomous Mobile Robot](../assets/images/projects/amr.jpeg)

Designed and implemented an **Autonomous Mobile Robot (AMR)** capable of mapping, localization, and navigation in indoor environments.

Key components:

- Built using **ROS 2, SLAM, and path planning frameworks**.
- Tested in **Gazebo simulation and real hardware setups**.
- Implemented **Cartographer SLAM, AMCL localization, and Navigation2 stack**.

**Repository:**  
[AMR GitHub](https://github.com/Sairamzz)

---

## APG-RRT Path Planner in ROS2

![APG RRT](../assets/images/projects/apgrrt.jpeg)

Implemented an **Adaptive Path-Guided Rapidly-Exploring Random Tree (APG-RRT)** planner for mobile robot navigation.

Key components:

- Adaptive sampling-based path planning algorithm.
- Evaluated performance across multiple **2D environments**.
- Integrated with **TurtleBot3 in Gazebo** using custom maps.
- Achieved **~25% faster path generation compared to baseline RRT**.

**Repository:**  
[Path Planner GitHub](https://github.com/Sairamzz)

---

## Structure-from-Motion (SfM) 3D Reconstruction

![SfM Reconstruction](../assets/images/projects/sfm.jpeg)

Implemented a full **Structure-from-Motion pipeline** to reconstruct 3D scenes and estimate camera poses from 2D images.

Key components:

- Feature matching and **epipolar geometry estimation**.
- **Triangulation and incremental camera pose estimation**.
- Global **bundle adjustment using GTSAM**.
- Validated reconstruction accuracy using **COLMAP calibration outputs**.

**Repository:**  
[SfM Pipeline GitHub](https://github.com/Sairamzz)

---

## Camera–LiDAR Extrinsic Calibration (On-the-Fly)

![Camera LiDAR Calibration](../assets/images/projects/calibration.jpeg)

Developed a pipeline to estimate the **6-DoF extrinsic transformation between camera and LiDAR sensors** during runtime.

Key components:

- Processed synchronized LiDAR point clouds and camera images.
- Extracted geometric features using **KD-Tree search and Canny edge detection**.
- Optimized the camera-LiDAR transform using **grid search and pose refinement**.
- Validated calibration results through **visual overlays and robustness tests**.

**Repository:**  
[Camera-LiDAR Calibration GitHub](https://github.com/Sairamzz)
