# VIO + Geo-Location Navigation for GPS-Denied UAVs

A Python-based autonomous navigation framework for **GPS-denied drone environments** that combines **Visual–Inertial Odometry (VIO)** with **map-based geo-location correction**.

The system estimates local drone motion using a monocular/RGB-D camera and IMU, then corrects long-term drift using known landmarks, geo-referenced maps, fiducial markers, UWB anchors, RF beacons, or visual place recognition.

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
