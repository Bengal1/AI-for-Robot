# AI-for-Robot
This is the final project of my B.sc in Elecrical engineering at Tel-Aviv University.
This project is part of a large project - Robot that purify airplane's cabin from viruses.
The project is Implemented with ROS and have some improvement to be done.

this project Implements RTAB-Map as well as Gmapping. I have found it to improve 2D mapping. the 2D mappinimg of RTAB-Map only is quite noisy and It make it difficult for the robot to navigate in the environment.

maybe something about corona virus

this package contains to the robot SLAM application and also the robot simulation.
#### Hygie - Real Robot SLAM
after installing if you will choose to udse thr real SLAM application

##### Hardware requierments:
1. single-board computers (SBC) - Nvidia Jetson, Raspberry Pi et cetera.
2. ***Camera***
3. Robot for implementation (optional).

## Related Publications:






## Installation Instructions
1. Install ROS - [ROS Installation Instructions](http://wiki.ros.org/melodic/Installation/Ubuntu)
2. Install ROS Navigation Package.
```shell
sudo apt-get install ros-melodic-navigation
```
  For more information go to [ROS-Navigation](http://wiki.ros.org/navigation)

3. Install Realsense Library for ROS.
  Installation of Intel realsense on Nvidia Jetson:[Jetson Installation Guide](https://github.com/IntelRealSense/librealsense/blob/master/doc/installation_jetson.md)
  For more information go to [RealSense](https://github.com/mahammadirfan/SLAM-using-intelrealsense-d435i)

4. Install RTAB-Map:
```shell
sudo apt install ros-melodic-rtabmap-ros
```
  For more information go to: [RTAB-Map-ROS](https://github.com/introlab/rtabmap_ros) 

5. Install ROS's Gmapping Package:
```shell
sudo apt-get install ros-melodic-gmapping
sudo apt-get install ros-melodic-navigation
sudo apt-get install python-opencv
sudo apt-get install python-numpy
sudo apt-get install python-scikits-learn
```
  For more Information go to [SLAM Gmapping](http://wiki.ros.org/slam_gmapping)

6. Clone this repository:
```shell
cd ~/catkin_ws/src/
git clone https://github.com/Bengal1/AI-for-Robot.git
cd ..
catkin_make
```

* (Optional) [RRT_Exploration](https://github.com/hasauino/rrt_exploration) Package.

### Requirement:



```
Common errors here : [COMMON ERRORS](https://github.com/edoardottt/READMENATOR/blob/master/COMMON_ERRORS.md)
