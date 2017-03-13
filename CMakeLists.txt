cmake_minimum_required (VERSION 2.6)
project (LM_Tutorial)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/Modules/")

find_package (Eigen3 REQUIRED)
include_directories (${EIGEN3_INCLUDE_DIR})

add_executable (LMOptimize main.cpp)

configure_file(measured_data.txt measured_data.txt COPYONLY)
