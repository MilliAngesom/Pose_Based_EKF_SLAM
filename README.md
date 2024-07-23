# Pose-based EKF SLAM for Robot Localization

## Overview
This project focuses on pose-based SLAM using an Extended Kalman Filter (EKF) for robot localization, specifically targeting a differential drive robot equipped with Lidar, IMU, and wheel velocity sensors. It utilizes the Iterative Closest Point (ICP) algorithm for mapping and state estimation within the SLAM framework. The system employs the Open3D library to manage point cloud registration operations, and the kobuki robot is used for simulation purposes, aiming to accurately localize a mobile robot using a LIDAR scanner.

## Prerequisites
Before running this project, ensure the following prerequisites are met:
- **ROS Neotic**: Ensure ROS Neotic is installed. Other ROS versions are also fine.
    ```bash
    export CATKIN_WS=~/catkin_ws/  # Set your Catkin workspace environment variable appropriately.
    ```
- **Open3D**: Ensure you have Open3D installed.
- **Stonefish Simulator**: Install Stonefish for simulation capabilities. Follow instructions at [Stonefish Documentation](https://stonefish.readthedocs.io/en/latest/install.html). After installation, clone and compile the ROS interface:
    ```bash
    git clone https://github.com/patrykcieslak/stonefish_ros ~/catkin_ws/src/
    ```
- **Additional Dependencies**: Follow installation guides for additional required packages in [turtlebot_simulation](https://bitbucket.org/udg_cirs/turtlebot_simulation/src/master/)

## Installation
To set up and run the project, follow these steps:

1. **Clone the Repository**

2. **Build the Project**

## Usage
- To launch the simulation, run:
    ```bash
    roslaunch turtlebot_simulation kobuki_basic.launch
    ```
- To start the SLAM node:
    ```bash
    rosrun pose_based_EKF_slam HOL_Final.py
    ```

## Video Demo
1. [Simulation Video](https://youtu.be/_t0QvoqK8oU)
2. [Real Robot Demo](https://youtu.be/YqAs7LerJx0)

## Paper
The detailed explanation of the project can be accessed [here](https://drive.google.com/file/d/1gejfjgUPDrHrL5meqoU4-hRMOq4SYv-u/view).
