# KUKA-LBR STACK with FRI

This repos are meant to be used together. The primary objective of this stack is to fill the void of a ROS based inferace for KUKA iiwa-lbr7/14. This uses KUKA's FRI (Fast Research Interface) to communicate with ROS. This is important in tasks that require fast update rates (~1000Hz).

## The repository organization is as follows
- **kuka_msgs** - Custom defined message types for dependancies
- **kuka_motion** - Repo for motion generation. P2P, Spline path generation
- **kuka_gazebo** - Gazebo simulation of KUKA LBR14
- **kuka_admm** - Optimal control with Differential Dynamical Programming

## Dependancies
- orocos-kdl- ```sudo apt-get install orocos-kdl``` or build from source
- Eigen3

## Steps to run the code
- This **kuka_ocp** contains sub modules. Once this is cloned, run ```git submodule init```
- Then to download other repos, run ```git submodule update``` 
