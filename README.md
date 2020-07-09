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
$ sudo apt-get install ros-kinetic-joint-state-controller
$ sudo apt-get install ros-kinetic-effort-controllers
$ sudo apt-get install ros-kinetic-position-controllers
$ sudo apt-get install ros-kinetic-robot-state-publisher
$ sudo apt-get install ros-kinetic-gazebo-ros-control
$ sudo apt-get install ros-kinetic-ros-control ros-kinetic-joint-state-controller ros-kinetic-effort-controllers ros-kinetic-position-controllers ros-kinetic-velocity-controllers ros-kinetic-ros-controllers ros-kinetic-gazebo-ros ros-kinetic-gazebo-ros-control
$ sudo apt-get install ros-kinetic-gazebo-ros-pkgs ros-kinetic-gazebo-ros-control
```

For production environments:

```sh
$ mkdir -p catkin_ws/src
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
$ cd catkin_ws/src
$ git clone https://github.com/Saytas/robotic_manipulator.git
Or Alternatively create a package
$ catkin_create_pkg "package_name" urdf

$ vi ~/rm_description/CMakeLists.txt
Add dependencies
find_package(catkin REQUIRED COMPONENTS
  urdf
  controller_manager
  joint_state_controller
  robot_state_publisher
)

$ vi ~/rm_description/package.xml
Add dependencies
<build_depend>controller_manager</build_depend>
  <build_export_depend>controller_manager</build_export_depend>
  <exec_depend>controller_manager</exec_depend>

  <build_depend>joint_state_controller</build_depend>
  <build_export_depend>joint_state_controller</build_export_depend>
  <exec_depend>joint_state_controller</exec_depend>

  <build_depend>robot_state_publisher</build_depend>
  <build_export_depend>robot_state_publisher</build_export_depend>
  <exec_depend>robot_state_publisher</exec_depend>
  
$ vi 
```

   [Ubuntu 16.04]: <https://releases.ubuntu.com/16.04/>
   [ROS]: <https://www.ros.org/>
   [Kinetic]: <http://wiki.ros.org/kinetic>
   
