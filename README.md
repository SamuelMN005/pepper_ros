# Pepper ROS
Alternative all-in-one repository for all Pepper ROS related packages. In this repository Pepper robot also works in a Gazebo simulation.

## Install
First install the dependecies which require this setting via apt
```sh
sudo apt-get install ros-kinetic-driver-base ros-kinetic-move-base-msgs ros-kinetic-octomap ros-kinetic-octomap-msgs ros-kinetic-octomap-mapping ros-kinetic-humanoid-msgs ros-kinetic-humanoid-nav-msgs ros-kinetic-camera-info-manager ros-kinetic-camera-info-manager-py ros-kinetic-vision-opencv ros-kinetic-cv-bridge ros-kinetic-moveit ros-kinetic-tf2-bullet ros-kinetic-tf2-sensor-msgs ros-kinetic-ros-control ros-kinetic-ros-controllers ros-kinetic-gazebo-ros ros-kinetic-gazebo-ros-control ros-kinetic-gazebo-plugins ros-kinetic-controller-manager ros-kinetic-ddynamic-reconfigure-python ros-kinetic-teleop-twist-keyboard
```

Then build the project
```sh
mkdir -p ~/pepper_ws/src
cd ~/pepper_ws/src
git clone git@github.com:SamuelMN005/pepper_ros.git
cd ~/pepper_ws
catkin_make
source devel/setup.bash
```

## Run Pepper teleop
In order to manipulate the base of the robot with the keybaord run the following command:
```commandline
rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=/pepper/cmd_vel
```

# Acknowledgment
Thank you to the following people for developing and modifying the code for making it work correctly:

https://github.com/awesomebytes
https://github.com/sasilva1998
