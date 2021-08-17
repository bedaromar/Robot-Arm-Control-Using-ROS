[Task1.pdf](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/files/7002834/Task1.pdf)
# Robot-Arm-Control-Using-ROS
**This is my first task in Robotics and AI department at SMART METHODS summer training, And In this file I'll explain the steps for using robot arm in ROS.

## Detailed Steps:

1- Download ORACLE Virtual machine from https://www.virtualbox.org
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.21.51.png)

2- Choose OS X host for mac
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.22.06.png)

3- After the download is complete, the program interface will appear as follows:
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.22.19.png)

4- Download Ubunto from https://ubuntu.com
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.22.31.png)

5- Go to the Download box, then Ubuntu Desktop, and finally choose 20.04 LTS
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.22.48.png)

6-Downloaded successfully.
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.23.02.png)

7-After opening the program to start working, I  faced several problems with the laptop because it has a low space, so I worked on the online ROS
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.23.14.png)


## Online ROS:
1- Create a new account from the following link: https://www.theconstructsim.com/rds-ros-development-studio/
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.23.31.png)

2- Creat a new project
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.23.41.png)

3- Install arduino_robot_arm package:

- Add the “arduino_robot_arm” package to “src” folder
	$ cd ~/catkin_ws/src
	$ sudo apt install git
	$ git clone https://github.com/smart-methods/arduino_robot_arm 

- Install all the dependencies 
	$ cd ~/catkin_ws
	$ rosdep install --from-paths src --ignore-src -r -y
	$ sudo apt-get install ros-melodic-moveit
	$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
	$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
	$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

- Compile the package
  $ catkin_make

![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.23.57.png)

4- Robot state publisher problem.
To solve this problem change ROS noetic to ROS kinetic and it will open
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.24.10.png)
![Circuit Diagram](https://github.com/bedaromar/Robot-Arm-Control-Using-ROS/blob/main/Simulation%20imgs/Screenshot%201443-01-10%20at%2001.24.23.png)


and now you can control and use the robot arm successfully ..
finally task is done 
