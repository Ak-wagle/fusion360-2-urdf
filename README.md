# fusion360-2-urdf (Fusion to URDF Conversion for SimpleBot)
Convert Autodesk Fusion 360 model - SimpleBot to URDF for seamless integration with ROS2 robotics framework.

## Introduction

This guide explains how to convert a Fusion 360 model of a SimpleBot to a URDF (Unified Robot Description Format) file. This process is essential for working with ROS2 (Robot Operating System 2) as it allows you to simulate and control your robot in environments like Gazebo. Converting your 3D model to URDF makes it compatible with ROS2 tools, enabling simulation, visualization, and robot control.

## Steps to Convert Fusion 360 Model to URDF

### Step 1: Prepare Your SimpleBot Model

Construct your bot or download the pre-modeled SimpleBot available in both `.f3d` and `.step` formats. Open your chosen file in Autodesk Fusion 360.

### Step 2: Clone the Fusion2URDF-ROS2 Repository

Open your terminal and execute the following command to clone the repository, or download it manually:

```bash
git clone https://github.com/dheena2k2/fusion2urdf-ros2.git
