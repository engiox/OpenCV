cmake_minimum_required(VERSION 3.23)
project(myApp)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(a ./motion_deblur_filter.cpp)

target_link_libraries(a ${OpenCV_LIBS})
