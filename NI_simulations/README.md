# Natural Intelligence Simulations

ROS packages for Natural Intelligence project H2020 simulations.

## Overview

The main simulation folders are:

##### first_goat

Simple first goat robot urdf model to simulate NI Integrator 3

- *goat_command* →
ROS package useful to command each goat joint through the [`plugin manager`](https://github.com/NMMI/ROS-Gazebo-plugin-qbmove)

- *goat_description* →
ROS package with the first goat urdf version with the floating base, 8 links and 8 joints
	
- *goat_gazebo* →
ROS package with folders and files useful to spawn the goat_robot in a Gazebo world

##### second_goat

Simulator of a quadrupedal robot modeled with a floating base and 8 qbmove advanced joints/links


- *second_goat_description* →
ROS package with the second goat urdf version with the floating base, 8 links and 8 joints actuated by qbmove advance
	
- *second_goat_gazebo* →
ROS package with folders and files useful to spawn the second goat_robot model in a Gazebo world

##### goat_plugin

Plugin used to implement searial elastic actuator in each model; it is fully explained [here](https://github.com/NMMI/ROS-Gazebo-plugin-qbmove)

- *sea_plugin* → ROS package to integrate a Serial Elastic Actuator for each joint
- *plugin_manager* → ROS package to easly manage joint control

## Getting Started

### Installing

To install the packages in this repo just clone it into your catkin_ws, make sure to clone also the external dependencies and then `catkin_make`.

### Running 

To run a simulation, launch the .launch file related to the selected environment, more details will be given inside each folder.
