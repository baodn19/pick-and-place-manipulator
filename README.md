<div align="center" style="text-align: center;">

<h1>Pick & Place Manipulator</h1>

<p>
  <b>A simulated MyCobot280 6 DOF manipulator for learning perception with the Point Cloud Library and motion planning with MoveIt2. Source: <a href="https://www.youtube.com/playlist?list=PLNWNEEf8BvG6lbOxH9AiXNetYcVgcJeWk">Automatic Addison</a></b>
</p>

![OS](https://img.shields.io/ubuntu/v/ubuntu-wallpapers/noble)
![ROS_2](https://img.shields.io/ros/v/jazzy/rclcpp)

</div>

## Overview
This repository contains ROS 2 packages for simulating and controlling the myCobot robotic arm using ROS 2 Control and MoveIt 2. It provides support for Gazebo simulation and visualization in RViz. Gazebo simulation also includes simulated 3D point cloud data from the depth camera (RGBD) sensor plugin for vision.

![Gazebo Pick and Place Task Simulation](https://automaticaddison.com/wp-content/uploads/2024/12/pick-place-gazebo-800-fast.gif)

![Pick and Place with Perception](https://automaticaddison.com/wp-content/uploads/2024/12/pick-place-demo-rviz-800-fast.gif)

## Features
- Gazebo simulation of the myCobot robotic arm
- RViz visualization for robot state and motion planning
- MoveIt 2 integration for motion planning and control
- Pick and place task implementation using the MoveIt Task Constructor (MTC)
- 3D perception and object segmentation using point cloud data
- Automatic planning scene generation from perceived objects
- Support for various primitive shapes (cylinders, boxes) in object detection
- Integration with tf2 for coordinate transformations
- Custom service for retrieving planning scene information
- Advanced object detection algorithms:
  - RANSAC (Random Sample Consensus) for robust model fitting
  - Hough transform for shape recognition
- CPU-compatible implementation, no GPU required. 
- Real-time perception and planning capabilities for responsive robot operation

![Setup Planning Scene](https://automaticaddison.com/wp-content/uploads/2024/12/creating-planning-scene-800.gif)

## Project Roadmap
- [ ] Switch to GPU implementation for optimized runtime
- [ ] Integrate the depth camera at the end effector for active perception
