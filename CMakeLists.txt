cmake_minimum_required(VERSION 2.8.3)
project(rospy_urdf_to_rviz_converter)

find_package(catkin REQUIRED)

catkin_python_setup()

###################################
## catkin specific configuration ##
###################################

catkin_package(
  CATKIN_DEPENDS rospy
)

#############
## Install ##
#############

install(PROGRAMS
  src/${PROJECT_NAME}/rospy_urdf_to_rviz_converter.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
