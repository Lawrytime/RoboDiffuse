ROS2 (Humble) Setup
=========================

##     Set locale

Make sure you have a locale which supports UTF-8. If you are in a minimal environment (such as a docker container), the locale may be something minimal like POSIX. We test with the following settings. However, it should be fine if you’re using a different UTF-8 supported locale.

    `locale  # check for UTF-8`

    `sudo apt update && sudo apt install locales`
    `sudo locale-gen en_US en_US.UTF-8`
    `sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8`
    `export LANG=en_US.UTF-8`

`locale  # verify settings`

## Setup Sources

You will need to add the ROS 2 apt repository to your system.

First ensure that the Ubuntu Universe repository is enabled.

`sudo apt install software-properties-common`
`sudo add-apt-repository universe`

Now add the ROS 2 GPG key with apt.

`sudo apt update && sudo apt install curl -y`
`sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg`

Then add the repository to your sources list.

`echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null`
