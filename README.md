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





























