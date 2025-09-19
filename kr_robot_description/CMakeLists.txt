cmake_minimum_required(VERSION 3.5)
project(kr_robot_description)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY 
  kr810/meshes kr810/urdf kr810/rviz
  DESTINATION share/${PROJECT_NAME}/kr810
)

install(
  DIRECTORY 
  blah/meshes blah/urdf
  DESTINATION share/${PROJECT_NAME}/blah
)

ament_package()
