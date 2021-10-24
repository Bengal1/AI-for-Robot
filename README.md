# AI-for-Robot
This is the final project of my B.sc in Elecrical engineering at Tel-Aviv University.
This project is part of a large project - Robot that purify airplane's cabin from viruses.
The project is Implemented with ROS and have some improvement to be done.

maybe something about corona virus

This package contains to the robot SLAM application and also the robot simulation.
#### Hygie - Real Robot SLAM
After installing if you will choose to udse thr real SLAM application, it's all in the Hygie folder.
**Hardware requierments:
1. single-board computers (SBC) - Nvidia Jetson Xavier NX or equivalent SBC.
2. RGB-D Camera with IMU - Intel RealSense D435i or equivalent combination. 
3. Robot for implementation (optional).
#### Purebot - Robot Ready Simulation
The purebot folder contains all the necessaries for simulating our robot. 
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

6. Install [Depth image to Laser scan converter](http://wiki.ros.org/depthimage_to_laserscan)

7. Clone this repository:
```shell
cd ~/catkin_ws/src/
git clone https://github.com/Bengal1/AI-for-Robot.git
cd ..
catkin_make
```

* (Optional) [RRT_Exploration](https://github.com/hasauino/rrt_exploration) Package.

## The Project:
#### Motivation/Objectives:
The coronavirus pandemic, is an ongoing global pandemic of coronavirus disease 2019 (COVID-19) caused by severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2). The novel virus was first identified in Wuhan, China, in December 2019, and it spread to other parts of mainland China and around the world. The World Health Organization (WHO) declared a Public Health Emergency of International Concern on 30 January 2020, and a pandemic on 11 March 2020. As of 3 October 2021, more than 234 million cases and 4.8 million deaths have been confirmed, making it one of the deadliest pandemics in history.
The motivation for the project stems from the health and economic need to rehabilitate the aviation industry that has experienced huge losses in the last two years, as well as reducing the mobility of the virus. These things that affect the public health and world economy.

This project Implements RTAB-Map as well as Gmapping. I have found it to improve 2D mapping. the 2D mappinimg of RTAB-Map only is quite noisy and It make it difficult for the robot to navigate in the environment.
### RTAB-Map vs RTAB-Map+Gmapping
We have found that combining RTAB-Map and Gmapping provides better 2D map then only RTAB-Map and do not eopardise the 3D mapping of the RTAB-Map which it excel at.
You may see the differance on the Real environment mapping and on simulation mapping:
#### Simulation Mapping:
![image](https://user-images.githubusercontent.com/34989887/138611701-9e079077-a8c5-4db5-8d57-673bbdc8acb0.png)

#### Real Environment Mapping:
![image](https://user-images.githubusercontent.com/34989887/138611711-fffd7097-48a7-4b45-b6d0-e486dc7aee8a.png)


