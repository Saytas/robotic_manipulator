# Robotic Manipulator

### Tech

Requirements for the open source project to work properly:

* [Ubuntu 16.04] - Ubuntu 16.04 LTS ('Xenial Xerus') is a long-term support release of Ubuntu. This means it is supported for 5 years with critical security, bug and app updates from Canonical, the company that makes Ubuntu.
* [ROS] - ROS is an open-source, meta-operating system for your robot. It provides the services you would expect from an operating system, including hardware abstraction, low-level device control, implementation of commonly-used functionality, message-passing between processes, and package management.
* [Kinetic] - ROS Kinetic Kame is the tenth ROS distribution release.

### Installation

```sh
$ sudo apt-get install ros-kinetic-octomap-rviz-plugins
$ sudo apt-get install ros-kinetic-rtabmap ros-kinetic-rtabmap-ros
$ sudo apt-get install ros-kinetic-rtabmap-ros
$ sudo apt-get install ros-kinetic-joint-state-publisher-gui
$ sudo apt-get install ros-kinetic-ros-control ros-kinetic-ros-controllers
$ sudo apt-get install ros-kinetic-ros-controller-manager
```

For production environments:

```sh
$ mkdir -p catkin_ws/src
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
$ cd catkin_ws/src
$ git clone https://github.com/Saytas/robotic_manipulator.git
```

   [Ubuntu 16.04]: <https://releases.ubuntu.com/16.04/>
   [ROS]: <https://www.ros.org/>
   [Kinetic]: <http://wiki.ros.org/kinetic>
   
