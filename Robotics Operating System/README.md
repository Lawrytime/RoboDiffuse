ROS2 (Humble) Setup
=========================


![](https://roboticsbackend.com/wp-content/uploads/2022/04/ros_logo.png)  ![](https://docs.ros.org/en/humble/_static/humble-small.png) 

## 

## `Setting up the ROS2 (Humble) Enviroment with the essential add-ons required to run RoboDiffuse on ROS2, Ubuntu 22.04`

### Content
- [Set locale](#set-locale)
- [Setup Sources](#setup-sources)
- [Install ROS 2 packages](#install-ros-2-packages)
- [Universal Robots ROS2 Driver](#universal-robots-ros2-driver)
- [ROS2 Control](#ros2-control)
- ✅✅✅


##     Set locale

    locale  # check for UTF-8

    sudo apt update && sudo apt install locales
    sudo locale-gen en_US en_US.UTF-8
    sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
    export LANG=en_US.UTF-8

    locale  # verify settings


## Setup Sources

Add the ROS 2 apt repository to your system.

    sudo apt install software-properties-common
    sudo add-apt-repository universe

Add the ROS2 GPG key with apt.

    sudo apt update && sudo apt install curl -y
    sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg

Add the repository to your sources list.

    echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null


## Install ROS 2 packages

Update your apt repository caches after setting up the repositories.

    sudo apt update
    sudo apt upgrade

### Desktop Install (Recommended): ROS, RViz, demos, tutorials.

    sudo apt install ros-humble-desktop

Development tools: Compilers and other tools to build ROS packages

    sudo apt install ros-dev-tools

## Environment setup

Sourcing the setup script

Set up your environment by sourcing the following file.

`source /opt/ros/humble/setup.bash`



## Sample: Talker-listener

In one terminal, source the setup file and then run a C++ talker:

    source /opt/ros/humble/setup.bash
    ros2 run demo_nodes_cpp talker

In another terminal source the setup file and then run a Python listener:

    source /opt/ros/humble/setup.bash
    ros2 run demo_nodes_py listener


# Universal Robots ROS2 Driver

![](https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/blob/main/ur_robot_driver/doc/installation/initial_setup_images/e-Series.jpg)

### [Humble Branch](https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver/tree/humble)

Install the driver using

    sudo apt-get install ros-humble-ur


## ROS2 Control

    sudo apt-get install ros-humble-ros2-control

    source /opt/ros/humble/setup.sh


### Further instructions to set up RVIZ to receive commmands will be appended as code updates are made.

## Thanks.

#        ✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅✅
