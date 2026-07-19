# rssaem_ws_VB

## VB Downloads

https://drive.google.com/drive/folders/1Gv7wL4yO8bz2hNs2UMNFfkE4pFHIHHSC?usp=drive_link

sudo apt update

sudo apt install ros-humble-gazebo-ros-pkgs

source /opt/ros/humble/setup.bash

ros2 launch gazebo_ros gazebo.launch.py


## 테스트

## test 1

### Robot Terminal

ros2 launch rssaem_bringup rssaem.launch.py

### Remote PC 

ros2 launch rssaem_bringup rviz2.launch.py

ros2 run rssaem_teleop teleop_keyboard

#---------------------------------

## test 2

### Robot Terminal

ros2 launch rssaem_bringup rssaem.launch.py

### Remote PC 

ros2 launch rssaem_cartographer cartographer.launch.py

ros2 run rssaem_teleop teleop_keyboard

ros2 run nav2_map_server map_saver_cli -f ~/map

#---------------------------------

## test 3

### Robot Terminal

ros2 launch rssaem_bringup rssaem.launch.py

### Remote PC

ros2 launch rssaem_navigation2 navigation2.launch.py map:=$HOME/map.yaml



