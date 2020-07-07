# Install-tutlebot 

To install the dependent packages run :

cd ~/catkin_ws/src/

git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git

git clone https://github.com/ROBOTIS-GIT/turtlebot3.git
cd ~/catkin_ws && catkin_make

TurtleBot3 has three models, you have to set which model you want to use before you launch
TurtleBot3 by add this line at the bottom of the file:

gedit ~/.bashrc
export TURTLEBOT3_MODEL=burger

2. to download the TurtleBot3 simulation files.

cd ~/catkin_ws/src/
git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
cd ~/catkin_ws && catkin_make
. To launch the virtual robot using Gazebo

First,launch TurtleBot3 in an empty environment by :

roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch
