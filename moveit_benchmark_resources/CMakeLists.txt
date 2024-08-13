cmake_minimum_required(VERSION 3.10.2)
project(moveit_benchmark_resources)
find_package(ament_cmake REQUIRED)

ament_package()

install(DIRECTORY config databases bag_files launch DESTINATION share/${PROJECT_NAME})
