cmake_minimum_required(VERSION 3.23)
project(myapp)

message("** Cmake build type : "${CMAKE_BUILD_TYPE})

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(myapp ./Smoothing.cpp)

target_link_libraries(myapp ${OpenCV_LIBS})
