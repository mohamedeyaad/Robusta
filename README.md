# Robusta
This repository contains a full description, simulation and navigation on Gazebo of the service robot "Robutsa".

# Localiztion
We rely on AMCL, a probabilistic localization system for a robot moving in 2D, which implements the adaptive Monte Carlo localization approach, it uses a particle filter to track the pose of a robot against a known map. The map is provided the map_server ROS Node, which offers map data as a ROS Service. Locomotion is provided by the move_base package providing an implementation of an action that, given a goal in the world, will attempt to reach it with a mobile base. The move_base node links together a global and local planner to accomplish its global navigation task.

# Mapping
We use the gmapping package which uses fast SLAM algoirthim to map perform a static map of the current environemnt by subscribing to the laser scan topic

# Path Planning
The goal of path planning is to navigate the robot in its environment to reach the specified goal taking into considerations the shortest, best path.

# Youtube Channel
https://www.youtube.com/channel/UCT82iOgs5BUqzbcCQr5Mo3Q

# Authors
* Mohammed Ashraf
* Mohamed Eyad
* Mohamed Alaa
