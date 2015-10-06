cmake_minimum_required(VERSION 2.8.3)
project(iai_office_sim)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
find_package(catkin REQUIRED COMPONENTS
  gazebo_ros
  
)
catkin_package(
  DEPENDS 
    gazebo_ros 
     
#  INCLUDE_DIRS 
#    include
)

include (FindPkgConfig)
if (PKG_CONFIG_FOUND)
  pkg_check_modules(GAZEBO gazebo)
endif()

