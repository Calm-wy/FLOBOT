# FLOBOT

[![Build Status](https://travis-ci.org/yzrobot/online_learning.svg?branch=master)](https://travis-ci.org/yzrobot/online_learning)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/85d6393df92749238fb740e173be5bfa)](https://www.codacy.com/app/yzrobot/online_learning?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yzrobot/online_learning&amp;utm_campaign=Badge_Grade)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[FLOBOT](http://www.flobot.eu/) is an EU funded Horizon 2020 project. The University of Lincoln is responsible for developing the human tracking for safety software module, and leadnig the environment reasoning and learning software module. In this repository, you find these two modules as a whole, and specifically:

* [bayestracking](\bayestracking) is a library originally developed by [Dr. Nicola Bellotto](http://webpages.lincoln.ac.uk/nbellotto/).

* [detector_msg_to_pose_array](\detector_msg_to_pose_array), [ground_plane_estimation](\ground_plane_estimation), and [upper_body_detector](\upper_body_detector) was originally developed for [STRANDS](http://strands.acin.tuwien.ac.at/) project.

* [bayes_people_tracker](\bayes_people_tracker) is also from [STRANDS ](http://strands.acin.tuwien.ac.at/) but adapted according to the [FLOBOT](http://www.flobot.eu/) needs.

* [flobot_tracker_bringup](\flobot_tracker_bringup), [object3d_detector](\object3d_detector), [pose_grid_map](\pose_grid_map), and [rgbd_leg_detector](\rgbd_leg_detector) are originally developed for [FLOBOT](http://www.flobot.eu/).

A detailed view of the proposed system in UML diagram is shown below:

![flobot_uol_uml.jpg](https://github.com/LCAS/FLOBOT/blob/master/flobot_uol_uml.jpg)

In which `leg_detector` and `people_msgs` can be found here: [https://github.com/wg-perception/people](https://github.com/wg-perception/people). For a more intuitive understanding, please refer to the following video.

[![YouTube](https://img.youtube.com/vi/H2dBDKZMFTE/0.jpg)](https://www.youtube.com/watch?v=H2dBDKZMFTE)

## Install & Build

Our system has been tested on Ubuntu 14.04 + ROS Indigo, as well as Ubuntu 16.04 + ROS Kinetic,  Let's take the latter as an example:

```bash
$ sudo apt-get install ros-kinetic-people*
$ sudo apt-get install ros-kinetic-velodyne*
$ cd catkin_ws/src
$ git clone https://github.com/LCAS/FLOBOT
$ cd ../catkin_ws
$ catkin_make
```

## Run
```bash
$ roslaunch flobot_tracker_bringup flobot_tracker.launch
```

## FLOBOT Perception Dataset

[http://lcas.github.io/FLOBOT/](http://lcas.github.io/FLOBOT/)

## Citation
If you are considering using this repository, please reference the following:

```
manuscript in preparation ...
```