# Installing the package arduino_robot_arm


Install the catkin to make a foulder on it:

`sudo apt-get install ros-noetic-catkin`


This is a folder called "catkin_ws" which we will install the package on it:

`mkdir -p ~/catkin_ws/src`


Enter to the folder:

`cd ~/catkin_ws/`


To install the package from the GitHub:

`catkin_make`

`cd ~/catkin_ws/src`

`git clone https://github.com/smart-methods/arduino_robot_arm`


To install the MoveIt, joint-state-publisher, and gazebo:

`cd ~/catkin_ws`

`rosdep install --from-paths src --ignore-src -r -y`

`sudo apt-get install ros-melodic-moveit`

`sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui`

`sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher`

`sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control`


To enter bashrc:

`sudo nano ~/.bashrc`


To change bash source:

`source /home/maha/catkin_ws/devel/setup.bash`


To update bashrc file source:

`source ~/.bashrc`


To run the robot arm:

`roslaunch robot_arm_pkg check_motors.launch`


To run the Move It:

`roslaunch moveit_pkg demo.launch`


To run Gazebo and Move It:

`roslaunch moveit_pkg demo_gazebo.launch`
