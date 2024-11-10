## Download ros2 humble
https://docs.ros.org/en/humble/Installation/Alternatives/Ubuntu-Install-Binary.html

# Install xacro pkg
sudo apt install ros-humble-xacro
# Install gazebo 
sudo apt install ros-humble-gazebo-ros-pkgs -y
# Create workspace
mkdir -p ~/dev_ws/src              #Create dev_ws folder and src folder inside
cd ~/dev_ws                        #Move to dev_ws folder
# Clone your repo in dev_ws/src
git clone <>
# Build your file
colcon build --symlink-install  
# Set up env
source install/setup.bash 



























## run on diff terminal
source ~/dev_ws/install/setup.bash                               #dev_ws is the name of the folder contain your project

colcon build --symlink-install  

ros2 launch my_bot rsp.launch.py                                 #launch before open gazebo and rviz

launch my_bot launch_sim.launch.py world:=obstacles.world        #create your own world with objects so that you you can test run your robot in gazebo then save only                                                                   objects(do not save the robot in the env) as file world in the config folder

rviz2                                                            #visual your robot to see what objects your robot scanned

ros2 run teleop.twist.keyboard teleop.twist.keyboard             #controll your robot manual



#Remember to check the other pkgs if you need and download them.

