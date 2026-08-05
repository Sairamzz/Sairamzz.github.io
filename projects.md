---
layout: default
title: Projects
permalink: /projects/
---

# Highlighted Project Works

---

# Robotics & Autonomous Systems

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
<i class="fa-brands fa-github"></i> APG-RRT Path Planner
</a>

---

## Three-Link Planar Biped Walking using Hybrid Zero Dynamics and Nonlinear Control

![Three-Link Planar Biped](../assets/images/projects/3linkbiped.jpeg)

Designed and implemented a **three-link planar biped** to study gait generation and closed-loop walking using **hybrid dynamics** and **nonlinear control**.

Key components:

- Derived the robot dynamics using the **Lagrangian** formulation and expressed them in manipulator form.
- Used **Hybrid Zero Dynamics (HZD)** for stable reduced-order walking gaits.
- Designed **Bezier polynomial-based virtual constraints** for joint trajectories.
- Optimized gait parameters using numerical optimization techniques (MATLAB's fmincon).
- Simulated walking behavior and analyzed stability using **phase portraits and Poincaré maps**.

**Project Repository:**  

<a class="repo-button" href="https://github.com/Sairamzz/Planar-Biped-Locomotion" target="_blank">
<i class="fa-brands fa-github"></i> 3-Link Biped Control GitHub
</a>

---
---

# Perception, Computer Vision & Localization

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
<i class="fa-brands fa-github"></i> SfM Pipeline
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
<i class="fa-brands fa-github"></i> Extrinsic Calibration
</a>

---

## Panoramic Image Stitching for Low-Contrast Images

![Panoramic Stitching](../assets/images/projects/panorama_low_contrast.jpeg)

Developed a computer vision pipeline for panoramic image generation from low-contrast image sequences using feature-based image alignment and stitching techniques.

Key components:

- Enhanced low-contrast images through preprocessing and contrast adjustment techniques.
- Detected and matched visual features across overlapping images.
- Estimated image transformations using homography and geometric alignment methods.
- Generated panoramic views through image warping and stitching.

**Project Repository:**

<a class="repo-button" href="https://github.com/Sairamzz/Panoramic-Image-Stitching-Low-Contrast-Images" target="_blank">
<i class="fa-brands fa-github"></i> Low-Contrast Image Stitching
</a>

**Related Work:** Implemented a similar panoramic image stitching pipeline for high-contrast image datasets.

<a class="repo-button" href="https://github.com/Sairamzz/Panoramic-Image-Stitching-High-Contrast-Images" target="_blank">
<i class="fa-brands fa-github"></i> High-Contrast Image Stitching
</a>

---
---

# AI - RL, ML, Neural Networks 

## Robotic Manipulation using SmolVLA (Physical AI Hackathon)

![VLA Robotic Manipulation](../assets/images/projects/VLA_Manipulator.png)

Developed a learning-based robotic manipulation pipeline using **LeRobot** and **SmolVLA** to enable autonomous food assembly with a Seeed reBot B601-RS robotic arm.

Key components:

- Collected teleoperated demonstrations to build a dataset for four manipulation skills including spatula grasping, fruit scooping, and yogurt dispensing.
- Trained and deployed a **SmolVLA** policy using the **LeRobot** framework for vision-based robotic manipulation.
- Integrated learned policies with robot perception to perform an end-to-end autonomous fruit yogurt assembly task.
- Demonstrated the complete manipulation pipeline at the **Physical AI Revolute Hackathon, August 2026**.

**Project Repository:**

<a class="repo-button" href="https://github.com/savieee/froyo_arm-" target="_blank">
<i class="fa-brands fa-github"></i> Robotic Manipulation using SmolVLA
</a>

---

## POMDP Navigation in MiniGrid

![RL POMDP](../assets/images/projects/rlminigrid.jpeg)

Implemented a navigation pipeline for partially observable MiniGrid tasks using reinforcement learning methods.

Key components:

- Formulated navigation as a **Partially Observable Markov Decision Process (POMDP)**.
- Implemented and compared **POMCP, PPO, and A2C** agents.
- Designed **observation encoding and history-based representations** for partial observability.
- Applied **reward shaping and exploration strategies** to improve learning efficiency.
- Evaluated performance across multiple environments with increasing complexity and stochasticity.

**Project Repository:**  

<a class="repo-button" href="https://github.com/Sairamzz/RL_MiniGrid" target="_blank">
<i class="fa-brands fa-github"></i> POMDP Navigation GitHub
</a>

---

## Parkinson's Disease Classification using Machine Learning

![Parkinson's Disease Classification](../assets/images/projects/Parkinsons.jpeg)

Developed a Parkinson's Disease classification pipeline using speech-derived biomarkers and supervised machine learning techniques.

Key components:

- Applied feature selection and preprocessing using acoustic speech features including jitter, shimmer, HNR, RPDE, and MFCCs.
- Trained and evaluated multiple machine learning models including KNN, SVM, Naive Bayes, Logistic Regression, Random Forest, AdaBoost, and Gradient Boosting.
- Compared model performance using Accuracy, Recall, F1-Score, and AUC metrics.

**Project Repository:**

<a class="repo-button" href="https://github.com/Sairamzz/Parkinsons-Disease-Classification" target="_blank">
<i class="fa-brands fa-github"></i> Parkinson's Disease Classification
</a>

---

## Fault Diagnosis of IC Engine Gearbox using Voting Classifiers

![Gearbox Fault Diagnosis](../assets/images/projects/Gearbox.jpeg)

Developed a machine learning framework for gearbox fault diagnosis using vibration signal analysis and ensemble voting classifiers.

Key components:

- Collected vibration data from healthy and defective gearbox systems under controlled operating conditions.
- Extracted statistical, histogram, and ARMA-based features from vibration signals.
- Implemented voting-based ensemble classifiers for automated fault detection and condition monitoring.

**Project Repository:**

<a class="repo-button" href="https://github.com/Sairamzz/ML-GearBox-Fault-Diagnosis" target="_blank">
<i class="fa-brands fa-github"></i> Gearbox Fault Diagnosis
</a>

---

## Clutch Fault Diagnosis using WiSARD Classifier

![Clutch Fault Diagnosis](../assets/images/projects/Clutch.jpeg)

Developed a clutch fault diagnosis framework using vibration signal processing, deep feature extraction, and WiSARD-based classification.

Key components:

- Converted vibration signals into image representations for machine learning analysis.
- Extracted discriminative features using pre-trained convolutional neural networks.
- Implemented a WiSARD classifier to identify multiple clutch fault conditions and component failures.

**Project Repository:**

<a class="repo-button" href="https://github.com/Sairamzz/ML-Clutch-Fault-Diagnosis" target="_blank">
<i class="fa-brands fa-github"></i> Clutch Fault Diagnosis
</a>
