# Notes

This is the notes that I take to put in my personal github, so that I can read it again for building whatever app in ROS 2

Initial Setup

'''
# Run this before anything, 
# this is to enable ROS 2 Environment in python

# bash
source /opt/ros/kilted/setup.bash
'''

Everything in ROS should be running now, just do this to create your repo

'''
# bash 

mkdir -p FILENAME/src
cd ~/FILENAME

ros2 pkg create --build-type ament_cmake --node-name NODE_NAME PACKAGE_NAME

colcon build --packages-select PACKAGE_NAME

'''