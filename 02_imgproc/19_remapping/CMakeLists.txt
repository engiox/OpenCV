cmake_minimum_required(VERSION 3.23)
project(myApp)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(a ./Remap_Demo.cpp)

target_link_libraries(a ${OpenCV_LIBS})
