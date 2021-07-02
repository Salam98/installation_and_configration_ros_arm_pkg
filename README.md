# installation_and_configration_ros_arm_pkg

1-	First we have to create a workspace using commands below :

$ source /opt/ros/melodic/setup.bash

$ mkdir  ~p ~/catkin_ws/src

$ cd ~/ catkin_ws/

$ catkin_make



2-	Second installing the package (Arduino_robot_arm)

$ cd ~/catkin_ws/src

$ sudo apt install git

$ git clone https://github.com/smart-methods/arduino_robot_arm

$ cd ~/ catkin_ws

$ rosdep install --from-paths src --ignore-src -r -y

$ sudo apt-get install ros-melodic-moveit

$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui

$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher

$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

$ catkin_make


3-	Launching (check_motors) on Rviz by the command:

$ roslaunch robot_arm_pkg check_motors.launch

![check_motors](https://user-images.githubusercontent.com/85636030/124302187-88512380-db69-11eb-96c9-734eef77e675.png)



4-	Launching (check_motors) on gazebo by the command:

$ roslaunch robot_arm_pkg check_motors_gazebo.launch

![gazebo](https://user-images.githubusercontent.com/85636030/124319711-5056da00-db83-11eb-838f-29da174c6e6a.png)



5-	moveIt in Rviz

$ roslaunch moveit_pkg demo.launch

![moveIt](https://user-images.githubusercontent.com/85636030/124319767-6a90b800-db83-11eb-8fe4-896ce1a47dbc.png)


6- moveIt in gazebo

$ roslaunch moveit_pkg demo_gazebo.launch

![moveItGazebo](https://user-images.githubusercontent.com/85636030/124319931-a3c92800-db83-11eb-8cfb-b969afd0d165.png)

