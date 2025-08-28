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
'''

Colcon build to basically build everything that we created

'''
# Colcon build to build everything 
colcon build --packages-select PACKAGE_NAME

'''


# Now, ROS2 but PYTHON REMIX LESGOO

see the .py files, especially publisher.py and subscriber.py. 

Those are the basic function that are the essential core of ROS itself, it has the message sent and read like usual. 


## After those are installed, we need to set some config files


Changes in package.xml
'''

<!-- ADDED -->
  <exec_depend> rclpy </exec_depend>
  <exec_depend> std_msgs <exec_depend>

<!-- END ADDED -->


'''

Changes in setup.py

# Added
# -------------------------------
'talker = py_pubsub.
publisher_member_function:main',
'listener = py_pubsub.
subscriber_member_function:main',

# END ADDED
# -------------------------------