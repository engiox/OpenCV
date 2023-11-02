cmake_minimum_required(VERSION 3.23)
project(myApp)

message("** Cmake Build Type : ${CMAKE_BUILD_TYPE}")

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(myApp ./Threshold.cpp)

target_link_libraries(myApp ${OpenCV_LIBS})
