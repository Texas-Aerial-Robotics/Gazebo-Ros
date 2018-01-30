# Gazebo-Ros
This repo is a ros package which couples our romba simulator to the ardupilot SITL sim as well as other ros-gazebo plugins

Please install the following dependencies to get the simulator to run

'''
 sudo apt install ros-kinetic-gazebo-ros ros-kinetic-gazebo-plugins
'''

## Instructions 

clone in Computations repo 

'''
 git clone https://github.com/Texas-Aerial-Robotics/Computations.git
'''

Add the following to your bashrc to use the roomba plugins

'''
export GAZEBO_MODEL_PATH=${GAZEBO_MODEL_PATH}:~/Computations/roomba_host/models
'''

'''
export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:~/Computations/roomba_host/build
'''


## To view camera plugin 
install image view 

'''
sudo apt install ros-kinetic-image-view
'''

To view camera footage 
'''
rosrun image_view image_view image:=/webcam/image_raw
'''

