cmake_minimum_required(VERSION 3.5)

project(dotnet_cmake_module NONE)

find_package(ament_cmake REQUIRED)

ament_package(
  CONFIG_EXTRAS "dotnet_cmake_module-extras.cmake.in"
)

install(DIRECTORY cmake
  DESTINATION share/${PROJECT_NAME})
