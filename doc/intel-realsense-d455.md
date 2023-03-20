# Intel RealSense Depth Camera D455

Model: https://www.intelrealsense.com/depth-camera-d455/.

ROS Wrapper: https://dev.intelrealsense.com/docs/ros-wrapper.

## ROS

Source:
https://github.com/IntelRealSense/realsense-ros/blob/ros1-legacy/README.md#installation-instructions.

### Configuration

1. Install the ROS package
   [realsense2_camera](http://wiki.ros.org/realsense2_camera)
   ```sh
   # Update OS
   sudo apt update
   sudo apt dist-upgrade

   #  Install ROS package
   sudo apt install ros-noetic-realsense2-camera ros-noetic-realsense2-description
   ```
2. Start the camera node (close the terminal > open it again)
   ```sh
   roslaunch realsense2_camera rs_camera.launch
   ```

**Note:** if your screen starts to rotate itself, it is due to the internal
Internal Measurement Unit (IMU) of the camera
([source](https://github.com/IntelRealSense/librealsense/issues/6941)). It seems
that Ubuntu detects automatically that an IMU is available, and then offers the
possibility of rotating the screen accordingly to the camera's orientation. A
work around is to disable the Ubuntu screen rotation:
top of the screen + arrow (where you turn off the screen) > _Lock Screen_
_Rotation_ (only appears when the camera is connected).


**Test:** Asus ROG G501VW (personal PC of Ricardo Sousa).

- Intel Core i7 6th Gen 6700HQ Quad-Core 2.60 GHz (up to 3.50 GHz)
- RAM 8G DDR4
- Nvidia GeForce GTX 960M 4GB DDR5
- 3 x USB 3.0, 1 x USB 3.1 Gen 2 (Type C)

### Examples

Source:
https://dev.intelrealsense.com/docs/ros-wrapper#ros-camera-nodes-examples.

**Note:** each example in the previous link has an explanation (click on the
column _Link to Example_ in the table!).

**Note:** rviz specific configurations of each launch file is available in the
current repository ([rviz configs](/hmi/rviz/)).
