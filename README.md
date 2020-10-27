# mybot_ws
This repo was cloned from : github.com/richardw05/mybot_ws

URDF model for Gazebo integrated with ROS

This repository includes : <br>
1) <strong>base</strong> - create simple URDF model <br>
2) <strong>base_sensors</strong> - add sensors to robot <br>
3) <strong>navigation</strong> - enable autonomous navigation (now updated for [ROS Melodic Morenia](http://wiki.ros.org/melodic))

For more information on running the code:  <br>
http://moorerobots.com/blog/post/6

# Our contribution
In the following we describe our contribution : <br>

1) Add a 'relaxed_astar' package that implements Relaxed A* algorithm, to replace the default base navigation algo.
2) Use of an empty map instead of a pre-computed one.
