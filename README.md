# Description #

This respository is an adaptation of ['stju_drone'] (https://github.com/NovoG93/sjtu_drone/tree/noetic) for ROS noetic. It is upgraded to allow multi drone spawn through urdf.xacro files.

# Requirements #
This package is compatible with ROS Noetic version (Ubuntu 20.04). Compatible with Gazebo 11
```
$ sudo apt-get install ros-noetic-desktop
```
# Download and Compiling #
```
$ cd <catkin_ws>/src
$ git clone https://github.com/jakkkobo/simple_drone
$ cd <catkin_ws>
$ catkin build
```

Here <catkin_ws> is the path of the catkin workspace. Please refer to the [tutorial](http://wiki.ros.org/ROS/Tutorials) about how to create a catkin workspace in ROS.

# Run
The simplest way is calling after you have built the workspace successfully.

```
$ cd <where you check out the code>
$ source devel/setup.bash
$ roslaunch sjtu_drone simple.launch
```
or
```
$ roslaunch sjtu_drone multi_uav.launch
```
# Running with keyboard
In second terminal:

```
$ rosrun sjtu_drone drone_keyboard
```
# Implementation - Multi UAV

![](https://github.com/jakkkobo/simple_drone/blob/master/multi_uav.png)


