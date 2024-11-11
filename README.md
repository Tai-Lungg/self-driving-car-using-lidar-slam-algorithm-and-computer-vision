# Download ros2 humble
https://docs.ros.org/en/humble/Installation/Alternatives/Ubuntu-Install-Binary.html

## Install xacro pkg
sudo apt install ros-humble-xacro

## Install gazebo 
sudo apt install ros-humble-gazebo-ros-pkgs -y

## Install teleop key
sudo apt install ros-humble-teleop-twist-keyboard

## Install twist_mux
sudo apt install ros-humble-twist-mux

## Install controller_manager 
sudo apt install ros-humble-ros2-control ros-humble-controller-manager

## Install ros2 control pkg
sudo apt-get install ros-humble-ros2-control

## Install robot state pub pkg
sudo apt-get install ros-humble-robot-state-publisher

## Install joint_state_publisher
sudo apt-get install ros-humble-joint-state-publisher

## Install sensor_msgs pkg
sudo apt-get install ros-humble-sensor-msgs

## Install slam toolbox pkg
sudo apt-get install ros-humble-slam-toolbox

## Install nav2 pkg
sudo apt-get install ros-humble-navigation2

## Install dependencies
sudo apt-get install ros-humble-rclcpp
sudo apt-get install ros-humble-ament-cmake
sudo apt-get install ros-humble-rclpy

## Create workspace
mkdir -p ~/dev_ws/src              #Create dev_ws folder and src folder inside
cd ~/dev_ws                        #Move to dev_ws folder

## Clone your repo in dev_ws/src
git clone <>

## Build your file
colcon build --symlink-install  

## Set up env
source install/setup.bash  #~/dev_ws$ source install/setup.bash 

## Run gazebo
ros2 launch my_bot launch_sim.launch.py world:=obstacles.world 





























