#  minimum required cmake version: 3.1.15 support vs2019

cmake_minimum_required(VERSION 3.1.15)
project(Sample-DepthUnitControl)

add_executable(DepthUnitControl DepthUnitControl.cpp)

set_property(TARGET DepthUnitControl PROPERTY CXX_STANDARD 11)
target_link_libraries(DepthUnitControl OrbbecSDK ${OpenCV_LIBS})

