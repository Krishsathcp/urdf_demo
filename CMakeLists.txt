cmake_minimum_required(VERSION 3.8)
project(urdf_demo)

find_package(ament_cmake REQUIRED)
find_package(robot_state_publisher REQUIRED)

install(
  DIRECTORY launch urdf
  DESTINATION share/${PROJECT_NAME}
)

ament_package()

