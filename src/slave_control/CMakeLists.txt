cmake_minimum_required(VERSION 2.8.3)
project(slave_control)

 find_package(catkin REQUIRED COMPONENTS
   gazebo_msgs
   gazebo_plugins
   gazebo_ros
   gazebo_ros_control
 )




catkin_package()
include_directories(
  ${catkin_INCLUDE_DIRS}
)
install(DIRECTORY config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
