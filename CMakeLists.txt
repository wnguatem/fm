cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(pcl_plane_segmentation_example)

find_package(PCL 1.2 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (pcl_plane_segmentation_example pcl_plane_segmentation_example.cpp)
target_link_libraries (pcl_plane_segmentation_example ${PCL_LIBRARIES}