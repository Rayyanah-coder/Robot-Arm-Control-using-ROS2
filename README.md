# Robot-Arm-Control-using-ROS2
this project contains ROS 2 packages and configurations for controlling a robotic arm using:  - `joint_state_publisher` and `Moveit and kinematics` for motion planning and kinematics
---

# Requirements :

-  ubuntu 22.04
-  ROS2 humble

---
# How to install
1- install all these pacakges :
```bash
sudo apt-get update && sudo apt-get install -y \
     ros-humble-joint-state-publisher-gui \
     ros-humble-gazebo-ros \
     ros-humble-xacro \
     ros-humble-ros2-control \
     ros-humble-ros2-controllers \
     ros-humble-joint-state-broadcaster \
     ros-humble-joint-trajectory-controller \
     ros-humble-controller-manager
     ros-humble-moveit \
     ros-humble-gazebo-ros2-control
```
2-clone the repo :
```bash
cd ~/ros2_ws/src
```
```bash
https://github.com/smart-methods/Robot_Arm_ROS2.git
```
3-build ( note : you may need to install the colcon command )
```bash
colcon build
```
4-source the project :
```bash
 install/setup.bash
```
---
# Controlling the robot arm by joint_state_publisher
to control the robotic arm by this method , add this line to the terminal :
```bash
ros2 launch arduinobot_description display.launch.xml
```
this windwo will show up : 
<img width="920" height="557" alt="Image" src="https://github.com/user-attachments/assets/96d37d06-71a3-43d8-9c47-df918f425114" />
---
# Controlling the robot arm by Moveit and kinematics
to control the robotic arm by this method , add this line to the terminal :
```bash
ros2 launch  arduinobot_mc demo.launch.py
```
this windwo will show up : 
<img width="1120" height="356" alt="Image" src="https://github.com/user-attachments/assets/c5dc7e24-f836-4cf9-bd7d-828458e2299f" />
---
# the difference between the two methods:
- see file [ Controlling_the_robot_methods.txt ]
---
# Credits
Project completed as part of the Smart Methods AI & Robotics Internship. @smart-methods
