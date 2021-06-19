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

These all program:

![Screenshot_2021-06-19_20-54-22](https://user-images.githubusercontent.com/71232960/122655542-babb5380-d15b-11eb-80e6-8243d0617304.png)

![Screenshot_2021-06-17_09-27-37](https://user-images.githubusercontent.com/71232960/122655587-0f5ece80-d15c-11eb-9535-e3a7de7c21d3.png)
![Screenshot_2021-06-19_20-59-45](https://user-images.githubusercontent.com/71232960/122655588-0ff76500-d15c-11eb-8051-952f6e429bba.png)

![Screenshot_2021-06-19_20-37-53](https://user-images.githubusercontent.com/71232960/122655592-1be32700-d15c-11eb-8213-ab62fcc043ab.png)
![Screenshot_2021-06-19_21-07-00](https://user-images.githubusercontent.com/71232960/122655595-1d145400-d15c-11eb-86b4-dd687dc950eb.png)
