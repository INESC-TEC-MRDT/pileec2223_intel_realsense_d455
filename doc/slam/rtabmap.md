# RTAB-Map

GitHub: https://github.com/introlab/rtabmap.

ROS Package: https://wiki.ros.org/rtabmap.

## ROS

### Installation

Source: https://github.com/introlab/rtabmap/wiki/Installation

```sh
# Update OS
sudo apt update
sudo apt dist-upgrade

#  Install ROS package
sudo apt install ros-noetic-rtabmap-ros ros-noetic-robot-localization ros-noetic-imu-filter-madgwick ros-noetic-octomap-rviz-plugins
```

## SLAM

Source: https://github.com/IntelRealSense/realsense-ros/wiki/SLAM-with-D435i.

### Launch

```sh
roslaunch realsense2_camera opensource_tracking.launch
```

**Note:** requires the calibration of the IMU!
(see hoe to calibrate Intel RealSense IMUs in
file:///home/sousarbarb/Downloads/Intel-RealSense-Depth-Cameras-IMU-Calibration-Tool.pdf)
