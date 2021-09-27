Pre requisite


mkdir -p ~/hector_group2_ws/src

cd ~/hector_group2_ws/

wstool init src https://raw.github.com/tu-darmstadt-ros-pkg/hector_quadrotor/kinetic-devel/tutorials.rosinstall

sudo apt install ros-melodic-gazebo-ros-control

sudo apt install ros-melodic-ros-control

sudo apt install ros-melodic-geographic-info

sudo apt install ros-melodic-joy

sudo apt install ros-melodic-teleop-twist-keyboard

sudo apt-get install libqt4-dev

catkin build


To test:

cd ~/hector_group2_ws

source devel/setup.bash

roslaunch hector_quadrotor_demo outdoor_flight_gazebo.launch

on another terminal:

rosservice call /enable_motors "enable: true"

rosrun teleop_twist_keyboard teleop_twist_keyboard.py






