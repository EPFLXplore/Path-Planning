# mybot_ws
This repo was cloned from : github.com/richardw05/mybot_ws

URDF model for Gazebo integrated with ROS

This repository includes : <br>
1) <strong>base</strong> - create simple URDF model <br>
2) <strong>base_sensors</strong> - add sensors to robot <br>
3) <strong>navigation</strong> - enable autonomous navigation (now updated for [ROS Melodic Morenia](http://wiki.ros.org/melodic))

For more information on running the code:  <br>
http://moorerobots.com/blog/post/6

You way also want to check out these video tutorials : <br>
https://www.youtube.com/watch?v=1aX7NFvKehs&list=PLPdFwncBNrd0mA9uOdKaTossDczzI_EQG&index=9

# Our contribution
In the following we describe our contribution : <br>

1) Add a 'relaxed_astar' package that implements Relaxed A* algorithm, to replace the default base navigation algo.
2) Use of an empty map instead of a pre-computed one.

To launch a typical simulation scenario, type in different consoles the following command lines :
1) Gazebo :
```console
$ roslaunch mybot_gazebo mybot_world.launch 
```
2) Navigation
```console
$ roslaunch mybot_navigation amcl_demo.launch 
```
Note that if you want to manually drive the robot around, the previous command can be replaced by :
```console
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py 
```
If this command doesn't work, make sure to install the 'teleop_twist_keyboard' package with :
```console
$ sudo apt-get install ros-noetic-teleop-twist-keyboard
```
3) Rviz visualization tool :
```console
$ roslaunch mybot_description mybot_rviz_amcl.launch 
```
