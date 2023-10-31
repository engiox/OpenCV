cmake_minimum_required(VERSION 3.24)

project(MyApp)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(myapp scan.cpp)
target_link_libraries(myapp ${OpenCV_LIBS})
