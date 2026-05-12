# VIO + Geo-Location Navigation for GPS-Denied UAVs

A Python-based autonomous navigation framework for **GPS-denied drone environments** that combines **Visual–Inertial Odometry (VIO)** with **map-based geo-location correction**.

![](https://github.com/1Px-Vision/VIO_Geo_Location/blob/main/mapping_Geo.jpg)

The system estimates local drone motion using a monocular/RGB-D camera and IMU, then corrects long-term drift using known landmarks, geo-referenced maps, fiducial markers, UWB anchors, RF beacons, or visual place recognition.

![](https://github.com/1Px-Vision/VIO_Geo_Location/blob/main/Geo_navigation_V1.gif)

---

## Overview

In GPS-denied environments, drones cannot rely on satellite positioning. This project provides a hybrid navigation pipeline that combines:

- **Visual–Inertial Odometry**
- **Geo-location correction**
- **Local mapping**
- **Obstacle-aware navigation**
- **Trajectory estimation**
- **Drone pose visualization**
- **Evaluation using RMSE and trajectory error**

The main objective is to answer two navigation questions:

### Proposed Navigation Architecture

```text
Camera Frames
     +
IMU Measurements
     ↓
Visual–Inertial Odometry
     ↓
CNN Deep Motion Prior
     ↓
Particle Filter Prediction
     ↓
Geo-Location Correction
     ↓
Fused Global/Local Pose
     ↓
GPS-Denied UAV Navigation
```

## Expected Improvement

Adding VIO + geo-location can improve:

Absolute scale estimation
Long-term trajectory drift
Return-to-home accuracy
Map-referenced navigation
Multi-agent coordination
Robustness in GPS-denied environments
Accuracy of final position and trajectory RMSE

![](https://github.com/1Px-Vision/VIO_Geo_Location/blob/main/Geo_Nav_1.gif)

<p align="center">
  <a href="https://github.com/1Px-Vision/VIO_Geo_Location/raw/main/Autonomous_Drone_Navigation_with_Deep_Learning_V2.mp4">
    ▶ Download / Watch Raw MP4
  </a>
</p>


![](https://github.com/1Px-Vision/UAV_DeepViO/blob/main/GPS_denied_forest_2.jpg)

<p align="center">
  <b>VIO + Geo-Location GPS-Denied Forest Navigation</b><br>
  Click the image to watch the Kapwing demo video.
</p>

<p align="center">
  <a href="https://www.kapwing.com/e/6a033f1f917c991a7529dd9d">▶ VIO + Geo-Location GPS-Denied Forest Navigation</a>
</p>
