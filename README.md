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
```

### Step 3: Copy the URDF Exporter Script

#### For Windows (PowerShell)

Open PowerShell and execute:

```powershell
cd <path to fusion2urdf-ros2>
Copy-Item ".\URDF_Exporter_Ros2\" -Destination "${env:APPDATA}\Autodesk\Autodesk Fusion 360\API\Scripts\" -Recurse
```

#### For Mac (zsh or bash)

Open your terminal and execute:

```bash
cd <path to fusion2urdf-ros2>
cp -r ./URDF_Exporter_Ros2 "$HOME/Library/Application Support/Autodesk/Autodesk Fusion 360/API/Scripts/"
```

### Step 4: Run the URDF Exporter Script in Fusion 360
In Fusion 360, navigate to `Utilities > ADD-INS > Scripts and ADD-INS`.
Find and run `URDF_Exporter_Ros2`.

### Step 5: Save the Description File

Save the generated description file in your preferred folder. This description package will contain necessary files, including a `.launch` file with `gazebo.launch.py`, which can be used to run your SimpleBot or any other 3D model in ROS2. These files allow for various tasks, such as:

- **Simulation**: Run and test your robot in Gazebo.
- **Visualization**: Use RViz to visualize your robot.
- **Control**: Develop and test control algorithms in ROS2.

You can also use the provided URDF file of SimpleBot directly in ROS2 for other tasks, such as:

- **Path Planning**: Test and develop path planning algorithms.
- **SLAM**: Implement Simultaneous Localization and Mapping.
- **Sensor Integration**: Integrate and test various sensors with your robot.

## Future Work

Instructions for running SimpleBot in Gazebo will be added soon.

## Acknowledgments

The instructions provided here, particularly those in Step 3, are based on the work from [Dheenadhayalan R's GitHub repository](https://github.com/dheena2k2). Please check out their repository for more details.



