cmake_minimum_required(VERSION 3.23)
project(myApp)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(a ./houghlines.cpp)
add_executable(b ./HoughLines_Demo.cpp)

target_link_libraries(a ${OpenCV_LIBS})
target_link_libraries(b ${OpenCV_LIBS})
