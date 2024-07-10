# Controlling-the-robot-arm
This repository describes how to control the robot arm by joint_state_publisher and Moveit. 

# Requirements 

1) Create and setup a catkin workspace by following this turtorial: https://www.youtube.com/watch?v=8uxd9RBQvmQ


2) Install the arudino_robot_arm package by following the steps/

   $ cd ~/catkin_ws/src

   $ sudo apt install git

   $ git clone https://github.com/smart-methods/arduino_robot_arm

3) Install the dependencies/ 

   $ sudo apt-get install ros-noetic-moveit

   $ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

   $ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

   $ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
   
  # Controlling the robot arm by joint_state_publisher
  
  - Run the following instructions/

    $ roslaunch robot_arm_pkg check_motors.launch
  - Result:
    
 ![joint1](https://github.com/ProShaden/Controlling-the-robot-arm/assets/174384069/714c8e0d-5b63-4ff9-99c2-753935335d03)

    $ roslaunch robot_arm_pkg check_motors_gazebo.launch
  - Result:

![joint2](https://github.com/ProShaden/Controlling-the-robot-arm/assets/174384069/eaf094b6-e350-4f25-99a0-19ab8446723f)

    $ rosrun robot_arm_pkg joint_states_to_gazebo.py
  - Result:

![joint3](https://github.com/ProShaden/Controlling-the-robot-arm/assets/174384069/9a070d30-7aad-4525-80a0-1d08c14d9911)

# Controlling the robot arm by Moveit and kinematics
- Run the instruction/

    $ roslaunch moveit_pkg demo_gazebo.launch
  
- Result:
  
  ![moveit](https://github.com/ProShaden/Controlling-the-robot-arm/assets/174384069/759cac88-14ec-48ef-aef4-84fa37238436)

