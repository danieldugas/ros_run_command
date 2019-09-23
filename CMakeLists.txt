cmake_minimum_required(VERSION 2.8.3)
project(ros_run_command)

find_package(catkin REQUIRED COMPONENTS
    rospy
)
catkin_package(
    CATKIN_DEPENDS rospy
)
install(PROGRAMS
    ros_run_command
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
